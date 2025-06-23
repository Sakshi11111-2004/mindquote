# 🧠 MindQuote - Emotion-Aware Quote Coach

MindQuote is an intelligent, mood-aware motivational quote assistant that uses AI and NLP to detect the user's emotion, retrieve the most relevant quote, explain its meaning in simple language, and generate a beautiful poster for inspiration.

---

## 🚀 Features

- ✅ Mood Detection using Hugging Face transformers
- 🔍 Semantic Quote Retrieval via RAG (Retrieval-Augmented Generation)
- 🧠 AI-Powered Quote Explanation using LLMs (Zephyr 7B or Flan-T5)
- 🎨 Poster Generator (with Pillow)
- 🖥️ Streamlit Frontend for interactive UI

---

## 🛠️ Tech Stack

| Component      | Technology                      |
|----------------|----------------------------------|
| Mood Detection | `distilbert-base-uncased` (HF)   |
| Vector Store   | Chroma + `all-MiniLM-L6-v2`      |
| LLMs           | `HuggingFaceEndpoint` (Zephyr-7B)|
| Poster Design  | Pillow (PIL)                     |
| UI             | Streamlit                        |
| Language       | Python 3.11                      |

---

## 🧪 How to Run Locally

### 1. Clone this repo

```bash
git clone https://github.com/yourusername/mindquote.git
cd mindquote

2. Install Dependencies

pip install -r requirements.txt
Make sure you have streamlit, langchain, transformers, chromadb, and Pillow.

3. Set Hugging Face Token (if not already)

huggingface-cli login
Or manually place your token in the code.

4. Launch App
streamlit run app.py
📁 Folder Structure
mindquote/
├── app.py
├── test_quote_ask.py
├── utils/
│   ├── quote_rag.py
│   ├── explain_quote.py
│   ├── mood_classifier.py
│   ├── poster_generator.py
├── quote_db/        # Chroma vector DB
├── poster.png       # Auto-generated poster
├── requirements.txt
📸 Sample Output
Mood: happy
Quote: "Happiness is not something ready made. It comes from your own actions."
✅ Poster saved as poster.png

💡 Future Ideas
🎤 Voice input

🌐 Web deployment (e.g. Streamlit Share, Hugging Face Spaces)

🎯 Personalized quote recommendation based on user history

📱 Android/iOS version (using Kivy or React Native)

🤝 Credits
Made with ❤️ by Sakshi Waghmare
Powered by Hugging Face, LangChain, and OpenAI

📄 License
This project is open source under the MIT License.
---

---

### ➕ Next Steps:

- Save this content as `README.md` in your `mindquote` folder
- Upload it to GitHub or commit via terminal:
  ```bash
  git add README.md
  git commit -m "Add project README"
  git push
