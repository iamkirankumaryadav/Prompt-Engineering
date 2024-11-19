# Google Prompting Essentials

### 5 Step Framework

A good prompt follows a simple framework.

### 1. Task (Personal, Format)
- You need to describe the task you want the GenAI tool to help you with.
- It should contain a **Persona** and a **Format** preference, so that the task is specific.
- Persona refers to what expertise you want the GenAI tool to draw from.
- You can ask the tool to take on a persona like a professional writer, or a marketing executive with 15 years of experience.
- You can ask it to create output for a specific audience, a customer, or a manager.
- You can be as detailed as you would like when adding a persona to your task.
- Format refers to how you want the output to appear, whether that's a bulleted list, summary, or table.

### 2. Context
- Necessary details to help the GenAI tool understand what you need from it.
  
### 3. References (Examples)
- Sometimes you will add references/examples for the GenAI tool to use while creating its output.
- With the help of examples the GenAI tool can give you a more useful output.
- There aren't always going to be clear references of what you need, especially when you are working on something more abstract.
- References give GenAI tools and examples to work from, and that can mean asking a GenAI tool to learn from the tone, style, or length of the reference provided.
- Providing multiple references/examples is also known as **few-shot prompting**. (Shot: Examples/References)
- Providing only one reference/example is known as **single-shot prompting**.
- Providing no references/examples is known as **zero-shot prompting**
- Between 2 to 5 references/examples is the sweet spot for a GenAI tool.
  
### 4. Evaluate
- Ask yourself if the input you provided gave you the desired/expected output.
  
### 5. Iterate
- If you evaluate and determine that you're not getting what you expect, you can try again by adding more information.

The order of how you construct a prompt is less important than the context of the prompt itself.

# Entire Story:
### 1. Specify the task
- Crafting a great prompt starts by describing the task you want the tool to help you with.
- The task is the foundation of any prompt.
- It’s what you’re asking the gen AI tool to do for you.
- Adding a task to your prompt is like writing a sentence asking someone to do something for you:
- Write a list. Draft a speech. Create an image.
- These are all tasks that a gen AI tool can help with.
- When you’re writing a task, you need to be clear and specific about what you want.
- If you write a task with vague instructions, it can result in an output that’s irrelevant or incorrect.
- To avoid that, give your tasks some specific details. That includes providing a persona and a format:
- Think of a persona as the expertise you want the gen AI tool to draw from.
- You can ask the tool to take on the perspective of a science expert or an industry analyst or ask it to create an output geared towards a specific audience, like your manager or team.
- The format is what you want the output to look like.
- Want a bulleted list? Or maybe a table so you can compare results side-by-side? Include those details in your task.


### 2. Include necessary context 
- When it comes to prompting, oversharing can be good.
- The more relevant details you include, the better your output will be.
- Providing lots of background information—like your goals, the reason for the task, or what you’ve tried before—rounds out the model's understanding of what you're looking for.
- These details are called context, and they’re a vital part of creating great prompts.
- For example, you could write:
- How was DNA discovered?
- Instead, write a prompt that includes detailed context or background information:
- You’re a science expert developing a new curriculum at a local college.
- Tell me in a couple of engaging paragraphs how DNA was discovered and what kind of impact it had on the world.
- Write it in a way that people unfamiliar with science would understand.
- You have gotten feedback from students that they found this course dry and unintelligible before, so you want to make sure that the explanation grabs the student's attention and makes a good first impression.

### 3. Provide references 
- References are examples or any additional resources that resemble what you want the gen AI tool to produce.
- Including references in a prompt is like showing your hairstylist an image of someone with the new haircut you’d like to try.
- Depending on the gen AI tool you’re using, you can include text, images, and even audio references to sharpen your input.
- Whether you share your own work or include external references, clearly identify how they fit into your overall objective so the gen AI tool understands exactly what to emulate.
- And no need to build an exhaustive set of references—two to five should be enough.
- For example, you could write:
- Write a product description for a watch like it’s in a magazine.
- Instead, write a prompt that provides relevant details, references two external resources, and identifies a format:
- Write a one-paragraph product description for a high-end watch with features like a scratch-resistant case and a water resistance rating of up to 30 meters.
- Base the description style on these examples from our website:
- Sunglasses: Our latest collection of handcrafted, heritage-inspired sunglasses features details like UV-protective lenses in shades specifically chosen to complement each frame—all at a price that won't break the bank.
- Plus, we made these sunglasses with vintage-inspired acetate frames and a keyhole bridge.
- Cardholder: Crafted in smooth Italian leather, this double-sided cardholder is designed to carry your cash and credit cards without the bulk of a full wallet.
- Fun fact: this cardholder is made in Naples, Italy, and will look great when you treat your friends to a round of summer spritzes."

### 4. Evaluate your output 
- Different AI models are trained on unique data and rely on different programming techniques.
- Some models may be better suited to specific uses like writing code or brainstorming ideas, while others might have limited outputs because of their training sets.
- No matter the model, running the same prompt multiple times will likely render different results because of how gen AI tools process data.
- That’s why it’s so important to evaluate your output.
- Before you use any AI-generated information, text, or materials, critically evaluate that the output is accurate, unbiased, relevant, and consistent before incorporating it into your workflows.
- If the output isn’t what you’re looking for, you should iterate on your prompt. 

### 5. Take an iterative approach 
- There will be times when your prompt simply isn’t leading to the output you need.
- That’s where our ABI advice comes in: Always Be Iterating.
- If you find an output lacking, continue clarifying what you need until it’s just right.
- The prompting framework sets you up to give gen AI tools the information they need to generate useful outputs—and it’s designed to apply across all kinds of tools and models.
- So whatever your gen AI tool of choice, make sure you specify your task, provide context and references, evaluate your outputs, and iterate your inputs. 
