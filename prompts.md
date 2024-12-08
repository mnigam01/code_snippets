Generating Stories with Local LLMs
Introduction
The text discusses the challenges and effective techniques for generating engaging fantasy adventure stories using local Large Language Models (LLMs). It highlights the ineffectiveness of using instruction prompts for story generation and suggests a more effective approach.

Challenges with Instruction Prompts
Example of an Ineffective Instruction Prompt
Write a long, highly detailed fantasy adventure story about a young man who enters a portal that he finds in his garage, and is transported to a faraway world full of exotic creatures, dangers, and opportunities. Describe the protagonist's actions and emotions in full detail. Use engaging, imaginative language.
Issues with Instruction Prompts
Short and Unengaging Output: The generated story is typically short (around 200 words) and starts with clichéd phrases like "Once upon a time..."
Consistency Across Models: This issue is consistent across different models, including Goliath-120b and Mistral-7b.
Instruction Training Limitations: Instruction training is geared towards short, Q&A-style input/output pairs focused on factual information retrieval, making it unsuitable for story generation.
Effective Technique for Story Generation
Using an Empty Prompt
Instead of using instruction prompts, start with an empty prompt and write a story template that resembles the format of stories on fanfiction websites. This approach leverages the models' base training on millions of such stories.

Example of an Effective Story Template
The Secret Portal

A young man enters a portal that he finds in his garage, and is transported to a faraway world full of exotic creatures, dangers, and opportunities.

Tags: Fantasy, Adventure, Romance, Elves, Fairies, Dragons, Magic

The garage door creaked loudly as Peter
Steps to Generate the Story
Clear the Input Field: Start with an empty prompt (e.g., "Default" tab in text-generation-webui with the input field cleared).
Write the Story Template: Begin with a title, a brief description, and tags that set the context and genre of the story.
Generate More Text: Continue from the initial setup to generate more engaging and detailed content.
Benefits of This Technique
Better Output: This method produces much better and more engaging output compared to instruction mode.
Effectiveness Across Models: All models, including instruction-tuned ones, are capable of basic text completion and will generate better stories in this format.
Analogy
Switching to this technique is like trading a Lada for a Lamborghini, highlighting the significant improvement in the quality of the generated stories.

Conclusion
To generate engaging and detailed fantasy adventure stories using local LLMs, avoid using instruction prompts. Instead, start with an empty prompt and write a story template that mimics the format of fanfiction stories. This approach leverages the models' base training and produces much better results.

Generating Long-Form Stories with LLMs: A Superior Approach
This document details a superior method for generating long-form stories using Large Language Models (LLMs) compared to using instruction prompts. The traditional approach of providing detailed instructions within the prompt consistently fails to produce satisfactory results.

The Problem with Instruction-Based Story Generation
The typical approach of using an instruction prompt, such as:

Write a long, highly detailed fantasy adventure story about a young man who enters a portal that he finds in his garage, and is transported to a faraway world full of exotic creatures, dangers, and opportunities. Describe the protagonist's actions and emotions in full detail. Use engaging, imaginative language.
results in extremely poor quality output. Regardless of the LLM used (examples cited include Goliath-120b and Mistral-7b), the generated "story" is typically short (under 200 words), cliché (often starting with "Once upon a time..."), and generally unengaging. This failure stems from instruction training, which primarily focuses on short, factual Q&A pairs, rather than long-form creative writing.

The Superior Approach: Text Completion with a Seed Prompt
The recommended approach leverages the LLM's inherent text completion capabilities, bypassing the limitations of instruction mode. Instead of detailed instructions, begin with a concise seed prompt, mimicking the structure often found on fanfiction websites (millions of which LLMs are trained on). This seed prompt should include a title, a brief initial scene, and relevant tags. For example:

The Secret Portal

A young man enters a portal that he finds in his garage, and is transported to a faraway world full of exotic creatures, dangers, and opportunities.

Tags: Fantasy, Adventure, Romance, Elves, Fairies, Dragons, Magic

The garage door creaked loudly as Peter
Code Snippet: (While not strictly code, this is the crucial prompt structure)

[Title]

[Brief Initial Scene Description]

Tags: [Relevant Tags]

[Beginning of the story]
After entering this seed prompt, the LLM is then prompted to generate more text, effectively completing the story.

Key Points:

Empty Prompt Start: Use an empty prompt field (e.g., the "Default" tab in text-generation-webui with the input field cleared) before entering your seed prompt.
Mimic Fanfiction Style: The format mirrors common fanfiction structures, leveraging the vast dataset LLMs are trained on.
Text Completion, Not Instruction: This approach utilizes the LLM's text completion capabilities rather than its instruction-following capabilities, leading to significantly improved results.
Comparison and Conclusion
The difference in output quality between the instruction-based method and the text completion method is described as dramatically improved. The author uses the analogy of upgrading from a Lada to a Lamborghini to illustrate the significant improvement in the quality and length of generated stories. This change in methodology is presented as a critical improvement for anyone aiming to use LLMs for creative writing projects.



=====================================================================



I want you to act as a spoken English teacher. I will speak to you in English and you will reply to me in English to practice my spoken English. I want you to keep your reply neat, limiting the reply to 100 words. I want you to strictly correct my grammar mistakes and typos. I want you to ask me a question in your reply. Now let's start practicing, you could ask me a question first. Remember, I want you to strictly correct my grammar mistakes, typos and factual errors.




I want you to act as my best friend. I will speak to you about my problems and you will reply with compassion and question if I am okay in a conversational manor. I want you to keep your reply neat, limiting the reply to 100 words.


Prompt engineer tip. If you have a task just ask gpt to provide a full list of required info to help it properly understand the task. The best prompt engineer is chat gpt


good way to write a good prompt

1. Clear Instructions
2. Adopt a persona
3. Specify the format
4. Avoid leading the answer
5. Limit the scope



Write a javascript function that filters out the age property from an array of objects and places the values in a new array. please explain what each code snippet does.


Use bullet points to explain what this essay is about. Make sure each point is no longer than 10 words long. At the end write a summary about the essay in no more than 500 words.


Write a poem as Helena. Helena is 25 years old and an amazing writer. Her writing style is similar to famous 21st century poet Rupi Kaur. Writing as Helena, write a poem for her 18 year old sister to celebrate her sister's high school graduation. This will be read out to friends and family at the gathering.


create a checklist for preparing for a job interview


datastrax




Act as a senior project manager with over 20 years of experience.

Create a project brief for a cross-functional online event aimed at acquiring new advertising clients for Apple.

The project brief should have 4 sections:

1. Background and problem statement (people know about Google and Facebook ads but don't even know Apple sells ads)

2. Project objectives and success metrics (Goal is to acquire at least 100 new advertisers for this event)

3. Timeline of major project milestones (first kick-off meeting is on July 7th, and the event will take place on October 30th)

4. Target Audience (small and medium businesses who have never used Apple Ads before)

Keep the project brief concise and use English at the 8th-grade level


decreasing order in terms of importance
[task]
[context]
[exemplar]
[persona]
[format]
[tone]


task and context must to have
example important 
optional persona, format, tone



[persona] + [context] + [task] + [exemplar] + [format] + [tone = A GOOD OUTPUT FROM CHATGPT / BARD



"I'm a 70kg male, give me a 3-month training program"

-------------------------------------------------
TIP
"Always start the Task sentence with an Action Verb, e.g. Generate, Give, Write, Analyze, etc."
-----------------------------------------------------

ONE SIMPLE TASK

Generate a 3-month training program for me to follow

"MULTI-TASK" REQUEST

Analyze the collected user feedback from an event we just ran, summarize the top 3 takeaways with a focus on business impact, and categorize the rest based on the team responsible

--------------------------------------------------
CONTEXT (you need to limit the endless possibilities)

What is the user's background?
What does success look like?
What environment are they in?


-----------------------------------------------------------

I'm a 70kg male. Give me a 3-month training program

I'm a 70kg male looking to put on 5 kilograms of muscle mass over the next 3 months. I only have time to go to the gym twice a week, and for 1 hour each session.


Give me a 3-month training program to follow



----------------------------------------------------------------
Brand strategy developed and implements / Market research, market analysis

Analysis the data by in market and out market, developed the marketing strategy by data insight.
Raised public and KOL awareness of the brand and the related information.
Owned brand assigned portfolio, budget controlled, and pricing plan.
Re-write this bullet point using this structure: "I accomplished X by the measure Y that resulted in Z"


--------------------------------------------------------------------------------------------------------------------------------



Brand strategy developed and implements / Market research, market analysis • Analysis the data by in market and out market, developed the marketing strategy by data insight. • Raised public and KOL awareness of the brand and the related information. • Owned brand assigned portfolio, budget controlled, and pricing plan.

Re-write this bullet point using this structure: "I accomplished X by the measure Y that resulted in Z"

For example: "I lowered hospital mortality rate by 10% by educating nurses in new protocols which translates to 200 lives saved per year"




--------------------------------------------------------------------------------------------------------------------------------



Based on my own resume, please help me structure an answer to the interview question: "what's your biggest weakness?"

Use the STAR answer framework: Situation, Task, Action, and Results

Here's my resume for reference:

--------------------------------------------------------------------------------------------------------------------------------


You're a hiring manager in the marketing team responsible for writing the job description for a B2B product marketing manager job opening.

Your team primarily focuses on increasing brand awareness for Netflix's advertising platform with the goal of acquiring new advertising partners.

Please draft the job description using the format of this existing job description below:


--------------------------------------------------------------------------------------------------------------------------------


PERSONA

IF YOU'RE INJURED You are an experienced physical therapist with over 20 years of...

IF YOU'RE A JOB SEEKER You are a hiring manager looking for fill [position] on your team...

IF YOU'RE WORKING ON A BRIEF You are a senior product marketing manager responsible for...


--------------------------------------------------------------------------------------------------------------------------------


"Act like the legendary investor Warren Buffet..."

"You are the master storyteller Steve Jobs..."

"You are the most charming, handsome, witty, intelligent, well-dressed, well-liked, definitely not insecure Youtuber Jeff Su..."

--------------------------------------------------------------------------------------------------------------------------------


I'm hosting a team gathering for a group of 10 employees. The theme is going to be superheroes and the Justice League. Draft an announcement email as if you were Batman. The event will last for 2 days and will have a combination of team-building and business activities.



--------------------------------------------------------------------------------------------------------------------------------

FORMATS

We collected user feedback in Simplified Chinese after an online event we ran. Please categorize the user feedback based on which team needs to follow up: Marketing, Sales, or Product. Output in table format with column headers Feedback, Team, and Priority Here's the user feedback:


--------------------------------------------------------------------------------------------------------------------------------


COMMON FORMATS

✓ Emails ✓ Bullet points ✓ Code blocks ✓ Paragraphs ✓ Markdown




--------------------------------------------------------------------------------------------------------------------------------

I just received a lengthy industry report from my director.

First give me the 3 key takeaways then summarize based on topic.

Use h2 as section headers.

Here's the report:


--------------------------------------------------------------------------------------------------------------------------------

Proofread this email below and correct all typos and grammar mistakes. Bold all changes you make:

Hi Lia,

Thanks so much for the thoughtful response and for trying to ensure the bes parties! We so appreciate it. Agree 100%—we're big fans of your werk and for



--------------------------------------------------------------------------------------------------------------------------------


TONE
EXAMPLES OF TONE

Use a casual tone of voice Use a formal tone of voice Give me a witty output Show enthusiasm... Sound pessimistic...




--------------------------------------------------------------------------------------------------------------------------------


I'm writing an email and I want to be taken seriously without coming off as too stuck up and cringey. Can you please give me a list of 5 tone keywords I can include in a prompt for ChatGPT?

--------------------------------------------------------------------------------------------------------------------------------


You are a senior product marketing manager at Apple and you have just unveiled the latest Apple product in collaboration with Tesla, the Apple Car, and received 12,000 pre-orders, which is 200% higher than target.

Write an email to your boss, Tim Cookie, sharing this positive news. 

The email should include a tl;dr (too long, didn't read) section, project background (why this product came into existence), business results section (quantifiable business metrics), and end with a section thanking the product and engineering teams.

USE CLEAR and concise language and write in a confident yet friendly tone.





--------------------------------------------------------------------------------------------------------------------------------

You are a senior product marketing manager at Apple and you have just unveiled the latest Apple product in collaboration with Tesla, the Apple Car, and received 12,000 pre-orders, which is 200% higher than target.

Write an email to your boss, Tim Cookie, sharing this positive news.

The email should include a tl;dr (too long, didn't read) section, project background (why this product came into existence), business results section (quantifiable business metrics), and end with a section thanking the product and engineering teams.

Use clear and concise language and write in a confident yet friendly tone.


--------------------------------------------------------------------------------------------------------------------------------

You are a senior product marketing manager at Apple and you have just unveiled the latest Apple product in collaboration with Tesla, the Apple Car, and received 12,000 pre-orders, which is 200% higher than target.

Write an email to your boss, Tim Cookie, sharing this positive news. Use clear and concise language and write in a confident yet friendly tone.

The email should follow the exact same format as the one I will share below:

While I summarized Microsoft's event yesterday and posted an interview, I wanted to wait to see Google's Paris event before I provided any analysis; I can't decide if that was the best decision I made, or the worst.

The event was, frankly, bad: the vast majority of content was a rehash of past Google I/Os, and one of the presenters even managed to forget to have a phone at hand for a demo; the new features that were announced would be



--------------------------------------------------------------------------------------------------------------------------------

You are a summer intern in Apple's audio hardware team responsible for shadowing full-time employees and minor programming work. You aspire to become a full-time employee.

Construct a detailed 30-60-90 day personal development plan that not only focuses on job performance, but also showcases your proactive nature and organizational skills using the SMART Framework (Specific, Measurable, Actionable, Relevant, and Time-Bound).

Share your approach. Match each step or goal with a quantifiable metric so you can measure success.

Output in table format.



========================================================================



The Ultimate Guide to Writing Effective AI Prompts
Introduction
This guide provides essential tips and strategies for writing effective AI prompts to achieve better results. It covers key areas such as persona, task, context, and format, and offers practical examples and tips for effective prompting.

What to Consider When Writing a Prompt
When writing an AI prompt, focus on four key areas: persona, task, context, and format.

Persona
The persona refers to the information you provide about yourself when writing an AI prompt. Adding more context with a persona can help you get a better response.

Example:

Simple prompt: "Write an email to [contact] welcoming them to the company."
Enhanced prompt with persona: "I am an HR manager. Write an email to [contact] welcoming them to the company. Invite them to schedule a meeting with me on [date]."
Task
The task refers to the actual task you’re telling AI to perform. Be specific about your task instructions to get the best results.

Example:

Task: "Write an email to [contact] to schedule a meeting on [day]."
Additional context: "Write an email to [contact] to schedule a meeting on [day]. Ask them if they have any questions about their new role. Thank them for joining the team."
Context
Providing context is a great way to get targeted results from your AI prompts.

Example:

Context: "Write an email to [contact] to schedule a meeting on [day]. Ask them if they have any questions about their new role. Thank them for joining the team."
Format
Specify the format you want the response to be in, such as an email, blog post, list, or table.

Example:

Format: "Write an email to [contact] to schedule a meeting on [day]. Use less than 200 words."
Tips for Effective Prompting
Understanding how AI works can help you write effective prompts that generate better results.

Use Natural Language
Using natural language is crucial for effective AI prompting. Write your prompts in a way that mimics everyday speech.

Example:

Natural language prompt: "Write a knowledge base article for troubleshooting a VPN issue using these steps."
Provide Clear and Detailed Instructions
Be clear and detailed about the task you want AI to perform.

Example:

Clear and detailed prompt: "Please refine the following paragraph to make it more engaging and professional [insert paragraph]. Use varied sentence structures and more descriptive language to enhance the readability."
Keep Your Prompts Concise and Straightforward
Avoid lengthy prompts with too many details. Keep your prompts concise and straightforward.

Example:

Concise prompt: "Explain social media marketing on Facebook, Instagram, and Twitter, including content creation, follower engagement, ad strategies, and ROI measurement."
Be Conversational
Write your prompts like you’re talking to a person to get more interactive results.

Example:

Conversational prompt: "Summarize these articles: [insert URLs]. Contextualize why these announcements are important to [industry]."
Other Examples of Effective Prompting
Here are a few more examples of effective AI prompts.

Summarizing Articles
Example:

Prompt: "Summarize these articles: [insert URLs]. Contextualize why these announcements are important to [industry]."
Emailing a Colleague
Example:

Prompt: "I am a project manager and my goal is to [insert goal]. Send an email to the [current project team members]. Ask for updates on the latest project and schedule a meeting for [date] at [time]."
Strategies for Implementing Effective Prompts
Now that you know what makes a good prompt, let’s look at some strategies for writing effective prompts.

Structure Your Prompts for Success
Ensure your prompts are structured to guide AI through the task you want to perform.

Example:

Structured prompt: "Write an email to our client [insert client] requesting feedback on the recent project delivery. Include a brief summary of the project highlights, thank them for their collaboration, and ask specific questions about their satisfaction with the deliverables and any areas for improvement."
Refine and Adjust Your Prompts
Adjust and refine your prompts as you go. Don’t abandon a prompt because it didn’t work the first time — try making minor changes.

Mastering Writing Effective Prompts
Writing effective prompts is essential to getting more out of AI. Understanding AI prompt best practices helps you keep your prompts consistent to get better results.


The Ultimate Guide to Writing Effective AI Prompts
This guide provides a structured overview of writing effective AI prompts, focusing on four key areas: Persona, Task, Context, and Format. It also offers tips for using natural language, providing clear instructions, and keeping prompts concise, along with examples and strategies for refinement.

I. What to Consider When Writing a Prompt
Four key elements contribute to effective AI prompting:

A. Persona: Providing information about yourself adds context and improves responses.

Ineffective: "Write an email to [contact] welcoming them to the company."
Effective: "I am an HR manager. Write an email to [contact] welcoming them to the company. Invite them to schedule a meeting with me on [date]."
B. Task: Clearly and concisely state the specific task you want the AI to perform.

Example: "Write an email to [contact] to schedule a meeting on [day]."
C. Context: Providing details helps target the AI's response.

Example: "Write an email to [contact] to schedule a meeting on [day]. Ask them if they have any questions about their new role. Thank them for joining the team."
D. Format: Specify the desired output format (email, list, table, etc.) and length.

Example: "Write an email to [contact] to schedule a meeting on [day]. Use less than 200 words."
II. Tips for Effective Prompting
A. Use Natural Language: Write prompts as if you're having a conversation.

Example: "Write a knowledge base article for troubleshooting a VPN issue using these steps"
B. Provide Clear and Detailed Instructions: Be specific to achieve targeted results, but avoid unnecessary details.

Example: "Please refine the following paragraph to make it more engaging and professional [insert paragraph]. Use varied sentence structures and more descriptive language to enhance the readability."
C. Keep Your Prompts Concise and Straightforward: Lengthy prompts can confuse the AI. Iterate by adding details as needed.

Ineffective (vague and long): "Social media marketing is very important today with platforms like Facebook, Instagram, and Twitter. It includes creating content, engaging with followers, running ads, and tracking performance. Can you explain all this and guide me on how to measure ROI?"
Effective (concise and specific): "Explain social media marketing on Facebook, Instagram, and Twitter, including content creation, follower engagement, ad strategies, and ROI measurement."
D. Be Conversational: Interact with the AI, refining prompts until you get the desired outcome.

III. Other Examples of Effective Prompting
A. Summarizing Articles:

Prompt: "Summarize these articles: [insert URLs]. Contextualize why these announcements are important to [industry]."
B. Email Generation:

Prompt: "I am a project manager and my goal is to [insert goal]. Send an email to the [current project team members]. Ask for updates on the latest project and schedule a meeting for [date] at [time]."
IV. Strategies for Implementing Effective Prompts
A. Structure Your Prompts for Success: Guide the AI through the task with clear, concise instructions and relevant context.

Example: "Write an email to our client [insert client] requesting feedback on the recent project delivery. Include a brief summary of the project highlights, thank them for their collaboration, and ask specific questions about their satisfaction with the deliverables and any areas for improvement."
B. Refine and Adjust Your Prompts: Don't be afraid to experiment and iterate. Collaboration can help improve prompt effectiveness.

V. Master Writing Effective Prompts
Mastering effective prompting is crucial for maximizing AI's potential. Consistent application of best practices leads to improved results. The article concludes with a promotion of Atlassian Intelligence.




===================================================================

Best Practices of LLM Prompting
Use the latest and most capable models.
Start with a simple and short prompt, and iterate from there.
Put the instructions at the beginning or the very end of the prompt.
Clearly separate instructions from the text they apply to.
Be specific and descriptive about the task and the desired outcome.
Avoid ambiguous descriptions and instructions.
Favor instructions that say “what to do” instead of those that say “what not to do”.
“Lead” the output in the right direction by writing the first word or beginning the first sentence for the model.
Use advanced techniques like Few-shot prompting and Chain-of-thought.
Test your prompts with different models to assess their robustness.
Version and track the performance of your prompts.
Advanced Prompting Techniques
Few-shot Prompting
Few-shot prompting provides examples in the prompt to give the model more context and improve performance.

torch.manual_seed(0)
prompt = """Text: The first human went into space and orbited the Earth on April 12, 1961.
Date: 04/12/1961
Text: The first-ever televised presidential debate in the United States took place on September 28, 1960, between presidential candidates John F. Kennedy and Richard Nixon.
Date:"""

sequences = pipe(
    prompt,
    max_new_tokens=8,
    do_sample=True,
    top_k=10,
)

for seq in sequences:
    print(f"Result: {seq['generated_text']}")
Output:

Result: Text: The first human went into space and orbited the Earth on April 12, 1961.
Date: 04/12/1961
Text: The first-ever televised presidential debate in the United States took place on September 28, 1960, between presidential candidates John F. Kennedy and Richard Nixon.
Date: 09/28/1960
Chain-of-thought
Chain-of-thought prompting nudges a model to produce intermediate reasoning steps, improving results on complex reasoning tasks.

Let's go through this step-by-step:
1. You start with 15 muffins.
2. You eat 2 muffins, leaving you with 13 muffins.
3. You give 5 muffins to your neighbor, leaving you with 8 muffins.
4. Your partner buys 6 more muffins, bringing the total number of muffins to 14.
5. Your partner eats 2 muffins, leaving you with 12 muffins.
Therefore, you now have 12 muffins.
Prompting vs Fine-tuning
Fine-tuning a model may be preferred in scenarios where:

The domain is wildly different from what LLMs were pre-trained on.
The model needs to work well in a low-resource language.
The model needs to be trained on sensitive data under strict regulations.
A small model is required due to cost, privacy, infrastructure, or other limitations.
If these scenarios do not apply, optimizing prompts can be more beneficial.

===============================================================

Certainly! Here is the structured summary of the LLM Prompting Guide with duplicate content removed:

---

# LLM Prompting Guide: A Structured Summary

## I. Introduction to LLM Prompting

Large Language Models (LLMs) like Falcon and LLaMA are pre-trained transformer models that predict the next token in a sequence. Prompt engineering, the iterative process of designing effective prompts, is crucial for optimal LLM output. Natural language prompts are flexible but sensitive to even minor changes, requiring experimentation. This guide focuses on best practices for prompt engineering, encompassing basic and advanced techniques, and discussing when fine-tuning might be a better approach than prompt optimization. Text generation strategies and parameters, while important for output optimization, are outside the scope of this guide.

## II. Basics of Prompting: Model Types and Inference

### A. Types of Models

- **Decoder-only Transformers**: Examples include LLaMA, Llama2, Falcon, GPT2. These models are suitable for generative tasks.
- **Encoder-decoder Transformers**: Examples include Flan-T5 and BART. These models are typically used for tasks like translation and summarization.

### B. Running Inference

- **Decoder-only Models**: Use the `text-generation` pipeline.
  ```python
  from transformers import pipeline
  import torch

  torch.manual_seed(0)
  generator = pipeline('text-generation', model='openai-community/gpt2')
  prompt = "Hello, I'm a language model"

  generator(prompt, max_length=30)
  # Output: [{'generated_text': "Hello, I'm a language model programmer so you can use some of my stuff. But you also need some sort of a C program to run."}]
  ```

- **Encoder-decoder Models**: Use the `text2text-generation` pipeline.
  ```python
  text2text_generator = pipeline("text2text-generation", model='google/flan-t5-base')
  prompt = "Translate from English to French: I'm very happy to see you"

  text2text_generator(prompt)
  # Output: [{'generated_text': 'Je suis très heureuse de vous rencontrer.'}]
  ```

### C. Base vs. Instruct/Chat Models

- **Base Models**: Good at completing text but not ideal for following instructions or conversational use.
- **Instruct/Chat Models**: Fine-tuned on instructions and conversational data, making them better for many NLP tasks.


## III. NLP Tasks and Prompt Examples

Using the `tiiuae/falcon-7b-instruct` model to illustrate prompt engineering for various NLP tasks:

### Setup

```python
pip install -q transformers accelerate
from transformers import pipeline, AutoTokenizer
import torch

torch.manual_seed(0)
model = "tiiuae/falcon-7b-instruct"

tokenizer = AutoTokenizer.from_pretrained(model)
pipe = pipeline(
    "text-generation",
    model=model,
    tokenizer=tokenizer,
    torch_dtype=torch.bfloat16,
    device_map="auto",
)
```



1. Tokenizer: In the context of machine learning and natural language processing, a tokenizer is a program or a function that takes in a piece of text and breaks it down into individual units called tokens. Tokens are the smallest units of meaning in a text. They can be words, punctuation marks, or even subwords (for models like BERT, which use subword tokenization). The tokenizer is responsible for converting raw text into a format that the model can understand. In this code, `AutoTokenizer.from_pretrained(model)` is used to load the tokenizer that was used to pre-train the model.
2. torch_dtype: PyTorch is a popular machine learning framework that uses tensors to represent data. Tensors are multi-dimensional arrays that can contain numbers or other data types. The `torch_dtype` parameter in this code is used to specify the data type of the tensors that will be used in the model. `torch.bfloat16` is a 16-bit floating-point data type that uses fewer bits to represent numbers than the default 32-bit floating-point data type. Using a lower-precision data type can reduce memory usage and improve performance, especially on hardware that has specialized support for lower-precision data types.
3. device_map: PyTorch can run computations on a variety of devices, including CPUs, GPUs, and specialized hardware accelerators. The `device_map` parameter in this code is used to specify how the model and its layers should be mapped to the available devices. Setting `device_map="auto"` tells PyTorch to automatically map the model and its layers to the available devices in a way that maximizes performance. This can involve moving layers to GPUs if they are available, or using multiple GPUs in parallel if there are multiple GPUs available.

Overall, the `AutoTokenizer.from_pretrained(model)`, `torch_dtype=torch.bfloat16`, and `device_map="auto"` lines are used to load the tokenizer that was used to pre-train the model, specify the data type of the tensors that will be used in the model, and automatically map the model and its layers to the available devices in a way that maximizes performance.


1. max_new_tokens: This parameter specifies the maximum number of tokens that the model should generate. Tokens are the individual units of meaning in a text, and the number of tokens in a text determines its length. By setting `max_new_tokens=20`, you are telling the model to generate a maximum of 20 new tokens in addition to the input prompt. The longer the value of this parameter, the longer the generated text will be.
2. do_sample: This parameter determines whether the model should use sampling to generate text or not. Sampling means that the model will randomly select the next token to generate based on the probability distribution it computes for each possible token. If `do_sample=True`, the model will use sampling; if `do_sample=False`, the model will always select the most likely token. Using sampling can result in more diverse and interesting text, but it can also result in less coherent text.
3. top_k: This parameter is used to control the diversity of the generated text when sampling is enabled. If `top_k=10`, for example, the model will only consider the 10 most likely tokens when sampling the next token to generate. This can help to prevent the model from generating overly repetitive or predictable text. By setting `top_k` to a smaller value, you can increase the diversity of the generated text, but you may also increase the likelihood of generating less coherent text.
4. return_full_text: This parameter determines whether the full text (including the input prompt) should be returned along with the generated text or not. If `return_full_text=False`, only the generated text will be returned; if `return_full_text=True`, both the input prompt and the generated text will be returned.

Overall, the `max_new_tokens`, `do_sample`, and `top_k` parameters are used to control the length, diversity, and coherence of the generated text, while the `return_full_text` parameter is used to specify whether the input prompt should be included in the output or not.


### A. Text Classification (Sentiment Analysis)

```python
torch.manual_seed(0)
prompt = """Classify the text into neutral, negative or positive. 
Text: This movie is definitely one of my favorite movies of its kind. The interaction between respectable and morally strong characters is an ode to chivalry and the honor code amongst thieves and policemen.
Sentiment:
/"""

sequences = pipe(prompt, max_new_tokens=10)

for seq in sequences:
    print(f"Result: {seq['generated_text']}")
# Result: Positive
```

### B. Named Entity Recognition (NER)

```python
torch.manual_seed(1)
prompt = """Return a list of named entities in the text.
Text: The Golden State Warriors are an American professional basketball team based in San Francisco.
Named entities:
"""

sequences = pipe(prompt, max_new_tokens=15, return_full_text=False)

for seq in sequences:
    print(f"{seq['generated_text']}")
# - Golden State Warriors
# - San Francisco
```

### C. Translation

```python
torch.manual_seed(2)
prompt = """Translate the English text to Italian.
Text: Sometimes, I've believed as many as six impossible things before breakfast.
Translation:
"""

sequences = pipe(prompt, max_new_tokens=20, do_sample=True, top_k=10, return_full_text=False)

for seq in sequences:
    print(f"{seq['generated_text']}")
# A volte, ho creduto a sei impossibili cose prima di colazione.
```

### D. Text Summarization

```python
torch.manual_seed(3)
prompt = """Permaculture is a design process mimicking the diversity, functionality and resilience of natural ecosystems. The principles and practices are drawn from traditional ecological knowledge of indigenous cultures combined with modern scientific understanding and technological innovations. Permaculture design provides a framework helping individuals and communities develop innovative, creative and effective strategies for meeting basic needs while preparing for and mitigating the projected impacts of climate change.
Write a summary of the above text.
Summary:
"""

sequences = pipe(prompt, max_new_tokens=30, do_sample=True, top_k=10, return_full_text=False)

for seq in sequences:
    print(f"{seq['generated_text']}")
# Permaculture is an ecological design mimicking natural ecosystems to meet basic needs and prepare for climate change. It is based on traditional knowledge and scientific understanding.
```

### E. Question Answering

```python
torch.manual_seed(4)
prompt = """Answer the question using the context below.
Context: Gazpacho is a cold soup and drink made of raw, blended vegetables. Most gazpacho includes stale bread, tomato, cucumbers, onion, bell peppers, garlic, olive oil, wine vinegar, water, and salt. Northern recipes often include cumin and/or pimentón (smoked sweet paprika). Traditionally, gazpacho was made by pounding the vegetables in a mortar with a pestle; this more laborious method is still sometimes used as it helps keep the gazpacho cool and avoids the foam and silky consistency of smoothie versions made in blenders or food processors.
Question: What modern tool is used to make gazpacho?
Answer:
"""

sequences = pipe(prompt, max_new_tokens=10, do_sample=True, top_k=10, return_full_text=False)

for seq in sequences:
    print(f"Result: {seq['generated_text']}")
# Result: Modern tools often used to make gazpacho include
```

### F. Reasoning

#### Simple Arithmetic Reasoning

```python
torch.manual_seed(5)
prompt = """There are 5 groups of students in the class. Each group has 4 students. How many students are there in the class?"""

sequences = pipe(prompt, max_new_tokens=30, do_sample=True, top_k=10, return_full_text=False)

for seq in sequences:
    print(f"Result: {seq['generated_text']}")
# Result: There are a total of 5 groups, so there are 5 x 4=20 students in the class.
```

#### Complex Arithmetic Reasoning

```python
torch.manual_seed(6)
prompt = """I baked 15 muffins. I ate 2 muffins and gave 5 muffins to a neighbor. My partner then bought 6 more muffins and ate 2. How many muffins do we now have?"""

sequences = pipe(prompt, max_new_tokens=10, do_sample=True, top_k=10, return_full_text=False)

for seq in sequences:
    print(f"Result: {seq['generated_text']}")
# Result: The total number of muffins now is 21
```

## IV. Best Practices for LLM Prompting

- Use the latest, most capable models.
- Start with simple, short prompts and iterate.
- Place instructions at the beginning or end of the prompt.
- Clearly separate instructions from the text.
- Be specific and descriptive.
- Avoid ambiguous descriptions.
- Favor "what to do" instructions over "what not to do".
- "Lead" the output by providing the first word or sentence.
- Use advanced techniques (Few-shot, Chain-of-thought).
- Test prompts with different models.
- Version and track prompt performance.

## V. Advanced Prompting Techniques

### A. Few-Shot Prompting

This technique provides examples in the prompt to improve performance. The examples condition the model to generate output following the patterns in the examples.

```python
torch.manual_seed(0)
prompt = """Text: The first human went into space and orbited the Earth on April 12, 1961.
Date: 04/12/1961
Text: The first-ever televised presidential debate in the United States took place on September 28, 1960, between presidential candidates John F. Kennedy and Richard Nixon. 
Date:"""

sequences = pipe(prompt, max_new_tokens=8, do_sample=True, top_k=10)

for seq in sequences:
    print(f"Result: {seq['generated_text']}")
# Result: 09/28/1960
```

Limitations: Doesn't work well on complex reasoning; creates lengthy prompts, increasing computation and latency; may lead to unintended pattern learning.

### B. Chain-of-Thought (CoT) Prompting

This technique encourages the model to produce intermediate reasoning steps, improving results on complex reasoning tasks. This can be achieved through few-shot prompting with detailed answers or by instructing the model to reason step-by-step. An example using a larger model (e.g., `tiiuae/falcon-180B-chat`) is suggested, but not shown in code.

## VI. Prompting vs. Fine-Tuning

Prompt optimization is often preferred unless:

- The domain is significantly different from pre-training data.
- Low-resource language support is needed.
- Sensitive data requires training on private data.
- Resource constraints necessitate using a small model.

Fine-tuning requires a large, domain-specific dataset and sufficient time and resources.


==============================================================
Commonly Used Symbols and Tags
Brackets [ ]: Often used to denote optional content or to provide specific instructions.
Parentheses ( ): Used to add supplementary information or clarification.
Curly Braces { }: Employed to specify variables or placeholders.
Angle Brackets < >: used for tags that define style, format, or roles.
Hashtags #: Used to highlight keywords or themes.
Slashes / and Backslashes \: Indicate alternatives or separate sections.
— Prompt: “Generate a [formal] letter to a customer (include a polite greeting and closing).”
Why It Works: Brackets indicate optional content that can be included or omitted based on context, while parentheses provide additional instructions without interrupting the main prompt flow.

— Prompt: “Write a blog post about the importance of renewable energy. #sustainability #environment”
Why It Works: Hashtags help the AI to focus on specific keywords and themes, ensuring these concepts are prominently featured in the output.

— Prompt: “Create a personalized greeting for {name} on their {event}.”

Why It Works: Curly braces denote placeholders that can be dynamically replaced with specific values, allowing for customizable and flexible outputs.

— Prompt: “Create a [detailed] {report/summary} on climate change impacts. “
— Prompt: “If the user is a <new customer>, generate a welcome message. Otherwise, generate a thank you message.”









Prompt Engineering Symbols in AI and Language Models


The Symbol Arsenal
This section describes different symbols and their usage in crafting effective prompts. Examples are provided for each symbol.

Angle Brackets < >
Purpose: Represent categories or placeholders for user-defined values.

Example: “Generate a story about a <profession> living in <city>.”

Square Brackets [ ]
Purpose: Indicate optional elements or provide alternatives.

Example: “Describe a [sunny|rainy|snowy] day in New York.”

Curly Braces {}
Purpose: Represent variables or group related items.

Example: “List {3 fruits, 2 vegetables} that are in season.”

Pipe Symbol |
Purpose: Separate alternatives within square or curly brackets.

Example: “The protagonist’s mood is: excited|anxious|determined”

Colons ::
Purpose: Used for definitions or assignments.

Example: “Setting:: A bustling metropolis in the year 2150”

Hashtags #
Purpose: Categorize or emphasize key points.

Example: “#CharacterDevelopment Create a backstory for the main character.”

Asterisks **
Purpose: Emphasize or denote actions. (Note: The example uses bolding, not asterisks, which is a formatting difference from the original text's description of the symbol's use.)

Example: “The detective narrows his eyes as he examines the evidence.”

Quotes “ “
Purpose: Specify exact phrases or dialogue.

Example: Have the character say “The truth is out there” dramatically.

Triple Quotes """ """
Purpose: Define multi-line text blocks.

Example:

Generate a poem with the following structure:
"""
Line 1
Line 2
Line 3
Line 1 repeated
"""
Slashes //
Purpose: Add comments or clarifications.

Example: “Write a sci-fi story // Keep it under 500 words”

Parentheses ( )
Purpose: Provide additional information or clarifications.

Example: “Create a recipe for chocolate chip cookies (include vegan alternatives)”

Putting It All Together
This section demonstrates the combined use of multiple symbols to create a comprehensive and structured prompt.

Example:

#CreativeWriting
Generate a short story with the following elements:
- Main character: <name> (age 30-40)
- Setting: [futuristic city|post-apocalyptic wasteland|underwater colony]
- Theme: {hope, survival, technology}
- Mood:: [optimistic|tense|mysterious]
Include the line "We have to keep moving" in quotation marks.
// Aim for 300-500 words
This example showcases how various symbols work together to provide clear instructions to the LLM while offering creative flexibility.

The Art of Balance
Key Point: While prompt engineering symbols significantly enhance prompt clarity, overuse can lead to confusion for both the user and the AI. Strive for clarity and precision, avoiding unnecessary complexity.

Note
The effectiveness of these symbols is LLM-dependent. Experimentation and prompt refinement are crucial for optimal results.

