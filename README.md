# 🤖 MemoryBot - Conversational AI Chatbot

Welcome to MemoryBot, an AI-powered conversational chatbot that uses Google's Gemini model to maintain and respond based on the context of previous interactions. This project leverages the capabilities of LangChain and Gradio to create an engaging and interactive chat experience.

## 📝 Overview

MemoryBot is designed to engage in meaningful conversations by remembering the history of interactions and generating responses that are contextually relevant. Whether you want to chat, ask questions, or simply interact with an AI, MemoryBot provides a friendly and intelligent response every time.

## 🚀 Features

- **Conversational Memory**: The chatbot remembers past interactions to generate context-aware responses.
- **Google's Gemini Model**: Utilizes Google's cutting-edge Gemini model for high-quality conversational abilities.
- **Customizable Responses**: Adjust the model's temperature and prompt template for different conversation styles.
- **Interactive Interface**: Built using Gradio for a user-friendly chat interface.

## ⚙️ How It Works

1. **Conversation History**: The bot maintains a history of all interactions using `ConversationTokenBufferMemory`, which allows it to remember and reference past conversations.
2. **Prompt Template**: A customizable prompt template guides the AI to generate creative, clever, and friendly responses.
3. **Response Generation**: The chatbot uses LangChain's `ConversationChain` to generate responses based on the user's input and conversation history.
4. **User Interaction**: Users can type messages, and the bot processes these inputs to generate appropriate responses that are displayed in the chat interface.

## 🛠️ Technologies Used

- **Gradio**: For building the interactive chat interface.
- **LangChain**: For managing the conversation flow and memory.
- **Google Generative AI**: For the underlying AI model (Gemini).
- **Python**: The primary programming language for this project.

## 🚀 Getting Started
   git clone https://github.com/majidhanif230/MemoryBot.git
   cd MemoryBot
   pip install -r requirements.txt
   python app.py
## 🙏 Acknowledgements
   This project was developed by Majid Hanif. Special thanks to Machine Learning 1 Pvt Ltd, the developers of LangChain and Gradio for their powerful tools, and the open-source community for their contributions.
