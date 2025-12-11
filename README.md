LLM Speech Summarizer using LangChain + Groq

This repository contains a complete demonstration of multiple summarization techniques using LangChain and Groq’s ultra-fast Llama models.
It shows how to summarize long speeches, PDFs, and multi-page documents using different state-of-the-art approaches.

Your included notebook:
📘 speech-summarize-groq.ipynb

🚀 Features
🔹 Summarization Techniques Included

Your notebook includes all major LangChain summarization approaches:

Summarization Type	Description
1. Simple Direct LLM Summarization	Quick summary using direct system & human messages.
2. Prompt-Template Based Summarization	Template-driven summarization + translation support.
3. Stuff Chain Summarization	Loads entire document (PDF) and summarizes in one go.
4. Map-Reduce Summarization	Splits long docs into chunks → summarize → combine into final summary.
5. Refine Chain Summarization	Creates an initial summary → updates it chunk by chunk for higher accuracy.

All five techniques are implemented inside your notebook.

📁 Project Structure

Your project (as visible in editor view):

LLM-SPEECH-SUMMARIZER/
│
├── .env.example                 # API key template
├── .gitignore                   # Ignore rules
├── apjspeech.pdf                # Sample PDF for testing
├── requirements.txt             # Python dependencies
└── speech-summarize-groq.ipynb  # Main notebook with all summarization methods

🔧 Setup Instructions
1️⃣ Clone this repository
git clone https://github.com/Shehjad2019/LLM-SPEECH-SUMMARIZER.git
cd LLM-SPEECH-SUMMARIZER

2️⃣ Create a Python virtual environment
python -m venv venv
source venv/bin/activate       # macOS / Linux
venv\Scripts\activate          # Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Add your Groq API key

Copy .env.example → .env:

cp .env.example .env


Then open .env and fill:

GROQ_API_KEY=your_actual_groq_api_key_here

💡 How to Use
▶️ Run Jupyter Notebook
jupyter notebook


Open:

speech-summarize-groq.ipynb

Inside the notebook, you can run:

✔️ Basic LLM summarization
✔️ Prompt-template summarization
✔️ Stuff summarization for smaller docs
✔️ Map-Reduce summarization for large PDFs
✔️ Refine chain for iterative summarization

PDF Example used:
📄 apjspeech.pdf

🧠 Technologies Used

LangChain (core, prompts, chains, loaders)

Groq ChatGroq Llama-3 models

PyPDFLoader for PDF parsing

RecursiveCharacterTextSplitter for chunking

dotenv for environment variable handling

Python 3.10+

🗂 Environment Variables

Stored in .env:

GROQ_API_KEY=your_groq_api_key_here

👤 Author

Shehjad Patel
GitHub: https://github.com/Shehjad2019

AI & Python Developer
