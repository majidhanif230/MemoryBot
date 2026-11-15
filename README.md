# MemoryBot

A conversational AI chatbot that remembers previous messages and replies in context, powered by Google's Gemini model (`gemini-pro`) with LangChain conversation memory and a Gradio chat interface.

> Project developed by Majid Hanif, with thanks to Machine Learning 1 Pvt Ltd.

## Key features

- Context-aware replies: `ConversationTokenBufferMemory` (max 1,000 tokens) keeps recent conversation history and drops the oldest tokens when the limit is reached
- Google Gemini (`gemini-pro`, temperature 0.7) via LangChain's `ChatGoogleGenerativeAI`
- Custom prompt template — the assistant is helpful, creative, clever, supportive and friendly
- Gradio `Blocks` web interface with a message box, Submit and Clear buttons

## Tech stack

- Python, Jupyter Notebook
- LangChain (`langchain`, `langchain-google-genai`)
- Google Generative AI (`google-generativeai`, Gemini)
- Gradio

## How to run

```bash
git clone https://github.com/majidhanif230/MemoryBot.git
cd MemoryBot
pip install -r requirements.txt.txt
```

Then open `MemoryBot.ipynb` in Jupyter and run the cells. Set your Google API key in the model-setup cell first — the notebook contains a placeholder where the key goes. (The requirements file in this repo is named `requirements.txt.txt`.)

There is no standalone `app.py` in this repo; the chatbot runs from the notebook, which launches the Gradio interface from its last cells.

## Project structure

```
MemoryBot/
├── README.md               # This file
├── MemoryBot.ipynb         # The chatbot: setup, memory, prompt, chain, Gradio UI
└── requirements.txt.txt    # gradio, langchain, google-generativeai, langchain-google-genai
```

How it works: user input goes through a LangChain `ConversationChain` built from the Gemini model, the token-buffer memory and the prompt template; the Gradio interface displays the reply and keeps the history for the next turn.

## Author

**Majid Hanif** — AI Engineer, BS Artificial Intelligence, The Islamia University of Bahawalpur (CGPA 3.81/4.0)

- Portfolio: https://snap-portfolio-me.lovable.app/portfolio
- LinkedIn: https://www.linkedin.com/in/majid-hanif-23720b2a2/
- GitHub: https://github.com/majidhanif230
