# Building blocks for a perfect prompt

### 1. Persona / Role
- Who should the AI be? Choose a role that matches your task, like Teacher, Doctor, Developer, Designer, Fitness Coach, etc.
- Assigning a role to the LLM, like **"You are a helpful assistant"** or **"You are a expert programmer."**
- Persona influences the style, context and content of the response.
- Eample: Want to build an app? Set the persona as a Developer. Creating a logo? Set the persona as a Graphic Designer.

### 2. Task / Instruction
- Always begin the sentence with an action verb and provide clear instructions with a defined goal.
- e.g., Generate, Give, Write, Draft, Analyze, Summarize, Translate, etc.
- The task may be a single, simple task or involve multiple requests.
- e.g., **Single / Simple Task:** Generate a 3-month workout plan.
- **Multiple Task Request:** Plan a Leh travel itinerary—search for the best places to visit, summarize the top three nearest my hotel, include accommodation and food options, and order them to minimize travel time.

### 3. Context
- What is the user's background? Provide relevant context or background information that the LLM can understand.
- Providing relevant background information or examples to guide the LLM's response.
- What does success look like? What is the user's aim? What environment are they in?
- Provide enough information to understand the context, aim, and objective to get accurate results.
- e.g., I am an 80kg male (background) looking to reduce 5kg of excess fat (success) over the next 3 months. I do not have time for the gym, so home workouts for 1 hour will be sufficient (environment).

### 4. Input Data / Output Indicator / Format
- Summarize the information the LLM should process (e.g., a text passage, a question, a code snippet).
- Visualize the exact format you want the result to look like.
- Specify the desired format or structure or type of the response (Text, list, code, etc)
- Define the desired output format or structure of the output (Paragraph, bullet points, table, code).
- **Formats:** Tables, emails, bullet points, code blocks, paragraphs, Markdown.

### 5. Constraints
- Limitations or rules the LLM must adhere to (e.g., "Keep the summary under 100 words," "Do not mention names").
- **Constraints:** Word counts, token limits, brevity, compactness, etc.
- **Rules:** Set any rules or guidelines the LLM should follow when generating output.
- **Example:** We collected user feedback, the sequence is First Name, Last Name, Contact, Email. Output in table format with specified column names.

### 6. Examples
- Showing the LLM some few shot examples where the reasoning process is explained in the examples.
- **Placeholders:** Create placeholders for specific information that will be filled in for each prompt instance. (e.g., Link and refereals: [text](url))
- The LLM will also show the reasoning process when answering the prompt.
- The explanation of reasoning often leads to more accurate results.
- e.g. Rewrite the bullet points using the STAR framework: Situation, Task, Action, and Results (Example Structure)
- Here is my resume for reference "Copy and paste your resume content"
- The examples are not necessary for every prompt but including a relevant example improves the quality of your output.

### 7. Tone
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

**You don't always need to use all 7 components.**

## Advanced Prompting Techniques:

### Few-Shot Prompting:
- Providing a LLM with few examples of input-output pairs to demonstrate the desired behavior.
- This helps the LLM understand the pattern you're looking for, leading to more accurate and relevant responses.
- LLMs are good at recognizing patterns. Few-shot prompting leverages this ability.
- It allows you to quickly adapt an LLM to specific tasks or styles without extensive training.

### Zero-Shot Prompting:
- Asking the LLM to perform a task without providing any examples.
- The LLM relies solely on its pre-existing knowledge gained during its training to understand and complete the task.
- LLMs are trained on vast amounts of text data, enabling them to understand various concepts and perform tasks without explicit examples.

### Chain-of-Thought (CoT) Prompting:
- Encouraging the LLM to break down complex problems into smaller, more logical steps, leading to a more accurate answer.
- Enhancing the reasoning abilities of LLMs by encouraging them to break down complex problems into a series of intermediate steps.
- Essentially, it guides the LLM to "think step-by-step" before providing a final answer.

### Tree-of-Thoughts (ToT) Prompting:
- Extending chain of thought prompting, and allowing the LLM to explore multiple reasoning paths, and then evaluate which one is the best before arriving at a solution.
- ToT enables LLMs to tackle complex tasks that require strategic planning and exploration of multiple possibilities.
- ToT allows LLMs to adapt to different problem-solving strategies and explore diverse solutions.

### Retrieval Augmented Generation (RAG):
- Retrieving relevant information from an external knowledge base and incorporating it into the prompt to enhance the LLM's response.
- Enhancing the capabilities of LLMs by allowing them to access and incorporate information from external knowledge sources. 
- This helps to address limitations such as outdated information or a lack of specific knowledge within the LLM's training data.
- RAG allows LLMs to "look up" information in real-time, making them more reliable and capable of providing up-to-date and accurate answers.

How RAG addresses these issues by:

1. **Retrieval:**
- When a user asks a question, the system first retrieves relevant information from an external knowledge base (e.g., a database, a document repository, or the internet).
- This retrieval process often involves converting the user's query and the knowledge base content into numerical representations (embeddings) and then finding the closest matches.

2. **Augmentation:**
- The retrieved information is then added to the user's prompt, providing the LLM with additional context.

3. **Generation:**
- The LLM uses both the original prompt and the retrieved information to generate a more accurate and informed response.

### Prompt Chaining:
- Breaking down a complex task into a series of simpler interconnected prompts, where the output of one prompt becomes the input for the next.
- Creating a "chain" of instructions that guide the language model towards the desired outcome.

### Iterative Prompting:
- Refining prompts based on the LLM's responses gradually improves the output quality.
- It is like having a conversation where you adjust your questions or instructions based on the LLM's response.
- By refining your prompts, you can significantly improve the quality and relevance of the LLM's output.

### System Prompt:
- A system prompt is a special type of prompt that's given to a LLM at the beginning of a conversation or interaction.
- It's used to set the overall tone, behavior, and guidelines for the LLM's responses throughout that session. Essentially, it defines the "role" or "personality" of the LLM.
- This ensure that the LLM maintains a consistent behavior throughout a conversation.

### Temperature:
- A parameter that controls the randomness of the LLM's output.
- **Higher** temperatures result in more creative, sometimes random and unpredictable responses.
- **Lower** temperatures produce more deterministic, consistent and focused responses.

### Top-p (Nucleus Sampling):
- A parameter that controls the diversity of the LLM's output by selecting from the most probable tokens until the cumulative probability reaches a certain threshold.

### Token:
- A basic unit of text that the LLM processes. It can be a word, a part of a word, a punctuation mark, or a full stop.

### Hallucination:
- When an LLM generates information that is factually incorrect or nonsensical.

### Grounding:
- Connecting the LLM's responses to reliable external sources to reduce hallucinations and improve accuracy.
- Example: RAG or providing access to a PDF, excel, word, or text file.

### Prompt Injection:
- A malicious technique where an attacker manipulates the LLM's behavior by injecting deceptive or wrong instructions into the prompt.

#### Do's and Dont's

**Do:**
1. Be clear and specific
2. Keep it conversational
3. Provide examples and guidance
4. Use correct punctuation, capitalization, and grammar
5. Be polite
6. Check for accuracy

**Don't:**
1. Don't just blindly copy and paste the responses. Validate the response.
2. Don't use slang words or jargons, keep your conversation professional and polite.
3. Don't provide conflicting instructions.
