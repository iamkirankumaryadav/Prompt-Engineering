# Building Blocks for a perfect prompt

### 1. Persona
- Who do you want the AI to be? Think of someone you wish to seek advice with the task you are facing.
- e.g. If you want to create a logo, a **graphic designer** will be the right person to set a persona.
- If you want to create a workout plan, a fitness expert will be the right person to set a persona.

### 2. Contextual Information (Context)
- What is the user's **background**? Provide relevant context or background information that the LLM can understand.
- What does **success** look like? Aim of the user? What **environment** are they in?
- Provide enough information to understand and get good results.
- e.g. I'm an 80kg male (background) looking to reduce 5kg of excess fat (success) over the next 3 months. I don't have time for the gym, so home workouts for 1 hour will be enough (environment).

### 3. Task Specification (Task)
- Always start the sentence with an **action verb** and provide instructions with a clear goal.
- e.g. Generate, Give, Write, Draft, Analyze, Summarize, Translate etc.
- The task can be **one simple task** or **multiple task request**.
- e.g. Simple Task: Generate a 3-month workout plan for me.
- Multiple Task Request: **Search** for the best places to visit in Leh, **summarize** the top 3 places nearest to my hotel, and **order** them so that it does not waste any time while travelling.

### 4. Examples
- Showing the LLM some few shot examples where the reasoning process is explained in the examples.
- Placeholders: Create placeholders for specific information that will be filled in for each prompt instance.
- The LLM will also show the reasoning process when answering the prompt.
- The explanation of reasoning often leads to more accurate results.
- e.g. Rewrite the bullet points using the STAR framework: Situation, Task, Action, and Results (Example Structure)
- Here is my resume for reference "Copy and paste your resume content"
- The examples are not necessary for every prompt but including a relevant example improves the quality of your output.

### 5. Format
- Visualize the exact format you want the result to look like.
- Specify the format or structure of the input (Text, list, code, etc)
- Define the desired output format or structure of the output (Paragraph, bullet points, table, code).
- Constraints: Word counts, number of tokens, brief, compact, etc.
- Rules: Set any rules or guidelines that the LLM should follow when generating the output. 
- e.g. We collected user feedback, the sequence is First Name, Last Name, Contact, Email. Output in table format with specified column names.
- Common Formats: Table, Emails, Bullet Points, Code Blocks, Paragraphs, Markdown.

### 6. Tone
- Style: Professional, Creative, Polite, Clear, Concise, Confident, Friendly, Formal, Casual, Request, etc.

### Prompt Example:

**Example 1:**
- You are a senior data scientist at Apple (Persona)
- You have received data for sales, which has the complete Business Requirement Document (Context)
- Write a professional email (Tone) to your team explaining to them the project background (Task)
- The email should be concise, including quantifiable business metrics, a section for objectives, key points, and results (Format with Example)

**Example 2:**
- You are a health and fitness expert (Persona)
- I'm a 75kg male looking to maintain muscle mass, I can go to the gym 5-6 days a week, and ideally for 50 minutes workout sessions (Context)
- Please give me a training plan based on the Push, Pull, Leg workout routine (Task)
- For example, a Push day includes 5-6 exercises aimed at the chest, shoulders, and back (Example)
- Output in a table format so I can easily paste it within a spreadsheet (Format)

**You don't always need to use all 6 components.**
