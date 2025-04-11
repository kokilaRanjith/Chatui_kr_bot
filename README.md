
### 🧠 Ollama + Streamlit Chatbot (Dockerized)

A fully local, lightweight chatbot interface powered by [Ollama](https://ollama.com) and built using [Streamlit](https://streamlit.io). This project is containerized with Docker for seamless deployment.


## 🚀 Features

- 🧠 Uses locally running LLMs via Ollama (e.g., Mistral, LLaMA2, etc.)
- ⚡ Fast, interactive UI with Streamlit
- 🔐 Private and offline-friendly
- 🐳 Containerized using Docker for portability


## 🛠️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ollama-streamlit-chatbot.git
cd ollama-streamlit-chatbot
```

### 2. Build the Docker Image

```bash
docker build -t ollama-chatbot .
```

### 3. Run the Docker Container

```bash
docker run -p 8501:8501 ollama-chatbot
```

> ✅ **Note**: Make sure you have [Ollama](https://ollama.com/download) installed and running on your machine before starting the container.

---

## 📄 Files Overview

| File             | Description                                  |
|------------------|----------------------------------------------|
| `simple.py`      | Main Streamlit app for chatbot (basic version) |
| `intermidate.py` | Alternative or extended version of chatbot app |
| `requirements.txt` | Python dependencies for the app              |
| `Dockerfile`     | Instructions to build the Docker image       |

---

## 🧪 Using Ollama Models

Before running the app, pull your desired model using Ollama CLI:

```bash
ollama pull mistral
```

Then, in `simple.py` or `intermidate.py`, update the model name if needed:

```python
response = ollama.chat(model="mistral", messages=chat_history)
```

---

## 📍 Access the App

Once the container is running, open your browser and navigate to:

```
http://localhost:8501
```

Start chatting with your private, local LLM!

---

## 🙌 Credits

- Built with [Streamlit](https://streamlit.io)
- Powered by [Ollama](https://ollama.com)
- Dockerized for easy sharing and deployment
```
