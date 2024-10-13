# Prompt Engineering

Crafting ideal inputs to get the most out of LLMs.

1. **Token:** A unit easily understood by a language model.
2. **Tokenization:** The mechanism to split the inputs into tokens.
3. **Completion:** The Language model takes a prompt and creates a completion by constantly predicting the next token.

### GPT
- **G:** Generative (Generated data)
- **P:** Pre-trained (Trained on a large amount of data)
- **T:** Transformer (Language model architecture)
- Support multiple modalities (Accept inputs in the form of image, text, audio, video)

### What makes GPT stand out?
- **Reinforcement learning from human feedback (RLHF)**
- Part of the model training where humans give feedback based on the model's response.

### Context Window
- The amount of tokens you can have in the input and output while interacting with the LLM.

### Biases
- GPT is trained on data from the internet and various sources, including 1000 of books and websites.
- Since, this are written by humans, some of these training data contains offensive information.
- That can cause gender, racial, and other biases.
- e.g. If you ask GPT about doctors and nurses, it considers doctors as male and nurses as female.
- Fine-tuning can help to decrease the bias.

### Gemini
- Gemini has a huge context window as compared to Chat GPT.
- Gemini offers Vertex AI to integrate the LLM into their applications.
- Gemini leverages the transformer's architecture and mixture of experts.
