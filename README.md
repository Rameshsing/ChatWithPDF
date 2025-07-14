
# 📄 Chat with PDF using Gemini

This project allows you to **chat with PDF files** using Google's **Gemini (Generative AI)** and **LangChain**. Upload your PDF files, ask questions, and get intelligent answers based on the document content.

---

## 🚀 Features

- Upload and process multiple PDFs
- Ask questions and get answers from PDF context
- Uses Gemini for text generation
- Uses FAISS for semantic search

---

## 🛠️ Installation & Setup

Follow the steps below to run this project locally on your machine:

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/chat-pdf-gemini.git
cd chat-pdf-gemini
```

Or simply download the code folder into your local system.

---

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
```

Activate the environment:

- **Windows**:
  ```bash
  venv\Scripts\activate
  ```

- **Linux/Mac**:
  ```bash
  source venv/bin/activate
  ```

---

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

---

### 4. Add Your Google API Key

Create a `.env` file in the root directory and add your **Google API Key**:

```
GOOGLE_API_KEY=your_google_api_key_here
```

You can get your API key from [https://makersuite.google.com/app](https://makersuite.google.com/app)

---

### 5. Run the Streamlit App

```bash
streamlit run chatpdf1.py
```

Then open your browser and go to:  
`http://localhost:8501`

---

## 📂 File Structure

```
chatpdf1.py             # Main Streamlit app
requirements.txt        # List of dependencies
.env                    # Your API key file (do not share this)
faiss_index/            # Auto-generated vector store (after processing PDFs)
```

---

## 📌 Notes

- Make sure your PDFs contain selectable/extractable text (not scanned images).
- Re-processing new PDFs will overwrite the old `faiss_index`.
- Avoid uploading large files if running on limited hardware.

---

## 🧼 License

This project is licensed under the Apache 2.0 License.
