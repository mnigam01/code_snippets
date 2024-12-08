current branch: main
command run git merge feature         

# bring all git commits in main branch from feature
# mai x branch par hu and mai git merge y se y ke changes la raha hu

----------------------------------------------

current branch : main
command git pull  or git pull origin main

# bring changes from github 
# mai x branch par hu and git pull krne se agar wo branch github par bhi hai toh uske latest changes la skta hu


---------------------------------------------------

current branch : feature
command run git pull origin main

# bring changes from github main branch into feature
# mai x branch par hu and git pull y se y ke saare changes x branch mai lekar aana chahta hu
# this is same as git checkout y > git pull > git checkout x > git merge y


----------------------------------------------------

current branch : feature
command run git rebase main

# bring all changes from main then change all commit from feature branch and show like a new commit is added after main latest changes
so something like main branch in a straight line followed by feature branch change

1. Context and Command Behavior:
Current Branch: feature
Command: git rebase main
Explanation:
When you are on the feature branch and you run git rebase main, Git temporarily moves all commits on feature that are not already on main to a temporary area.
Then, it updates your feature branch to point to the latest commit on main.
Finally, Git re-applies the commits from the temporary area one by one onto the updated feature branch, effectively placing them "on top" of the main branch's latest changes.
Result:
The history of feature is rewritten so that it appears as though your changes on feature were made after the latest changes on main.
This gives you a "linear" history where all main changes are followed by feature changes, as if the feature changes were introduced sequentially after the main branch’s latest state.



----------------------------------------------------

current branch : main
command run git rebase feature
# bring all changes from feature branch first, then apply changes from main branch on top of it.
# so let say main has 1>2>3>4>5 and feature has 1>2>10>11>12. The result will look like this
# 1>2>10>11>12>3'>4'>5' 


-----------------------------------------------------

scenario working on branch called feature, due to some requirement need to switch to feature2 branch. I have done some work
in feature branch. I can't switch branch due to work present. What are my options here?
1. Should I commit changes
2. Should I stash these changes

When should I prefer one over other?

Great question! When you have uncommitted work on your `feature` branch and you need to switch to `feature2`, you have two main options: **committing the changes** or **stashing them**. Let's go over when and why you might prefer one option over the other:

---

### 1. **Committing the Changes**
- **Description:** This means you create a new commit in the `feature` branch with your current changes before switching to `feature2`.
- **Use When:**
  - Your changes are in a relatively good state and represent a meaningful step in your work.
  - You are okay with adding a temporary or "work-in-progress" (WIP) commit to your branch history. These commits can later be amended, squashed, or rebased as needed.
  - You want to ensure that your changes are **saved in the version history** and are recoverable even if something goes wrong later.
- **Advantages:**
  - Creates a "snapshot" of your work that you can always go back to.
  - If you accidentally lose data or make mistakes while switching branches or working on `feature2`, your work on `feature` is saved.
- **Disadvantages:**
  - It may add noise to the commit history, especially if it’s not a finished or meaningful piece of work.
  - You may need to tidy up the commit history later (e.g., by using an interactive rebase).

**Good Practice:** If you go this route, consider using meaningful commit messages like "WIP: [Description]" to denote that it is an intermediate step.

---

### 2. **Stashing the Changes**
- **Description:** `git stash` temporarily saves your changes without committing them to the branch. It creates a "stash" entry that you can later apply and continue working on.
- **Use When:**
  - You are working on changes that are **not ready to be committed** and should not appear in the branch's commit history yet.
  - The changes are exploratory, incomplete, or not yet logically cohesive to become part of a commit.
  - You want a clean working directory to switch to another branch quickly without adding "noise" to your commit history.
- **Advantages:**
  - Keeps your branch's commit history clean and tidy.
  - You can easily restore your work after switching back to the `feature` branch using `git stash apply` or `git stash pop`.
  - You can create multiple stashes if needed and manage them using `git stash list`.
- **Disadvantages:**
  - It is temporary storage; if misused (e.g., forgetting to apply or pop a stash, creating too many stashes), you may risk losing track of your changes.
  - You need to remember to reapply your stashed changes when you switch back.

**Good Practice:** Always check your stash list (`git stash list`) to avoid forgetting about stashed changes.

---

### **When to Prefer Each Option:**

#### Prefer Committing When:
- Your changes are coherent enough to justify a new commit.
- You want the assurance of having a permanent record of your work.
- You anticipate being away from the branch for an extended period or need to push your work to a remote repository for sharing/collaboration.

#### Prefer Stashing When:
- Your changes are incomplete or experimental and don't represent a coherent unit of work.
- You want to maintain a clean history and plan to continue developing the same changes soon.
- You need to switch branches quickly without worrying about creating temporary commits that may clutter history.

---

**Example Workflow:**
1. **Stash Workflow:**
   ```bash
   git stash           # Save your uncommitted work
   git checkout feature2  # Switch to the other branch
   # Work on feature2
   git checkout feature  # Switch back to feature
   git stash apply       # Reapply your stashed changes
   ```

2. **Commit Workflow:**
   ```bash
   git add .                  # Stage your changes
   git commit -m "WIP: [description]"  # Create a WIP commit
   git checkout feature2      # Switch to the other branch
   ```

### **Conclusion:**
- **For quick, temporary work** or if you want to keep a clean commit history, **stashing** is generally better.
- **For saving changes as part of a permanent record**, **committing** is the way to go.
