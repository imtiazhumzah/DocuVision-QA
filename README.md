# DocuVision-QA
# 📘 DocuVision QA — Multimodal RAG over PDFs

DocuVision QA is a **retrieval-augmented assistant** that can **answer questions over technical PDFs** containing **text, tables, and figures**.  
It uses a **multimodal RAG pipeline** (text + image) with dual indexes and fusion retrieval for grounded answers.

---

## 🚀 Features
- 📑 Extracts **text, tables, figures, and captions** from PDFs
- 🔍 Builds **dual indexes** (textual + visual embeddings)
- 🔗 **Fusion retrieval** (text + image retrieval combined)
- 🧠 **Cross-encoder reranking** for precise results
- 📌 Returns **answers with citations and highlighted snippets**
- 🛠 Powered by **LlamaIndex + Hugging Face + PyMuPDF + OCR**

---

## 📂 Project Structure
- `notebooks/docuvision_qa.ipynb` → Main Colab notebook
- `src/data_loader.py` → PDF parsing (text, tables, images)
- `src/index_builder.py` → Dual index construction
- `src/retriever.py` → Fusion retrieval + reranking
- `src/qa_pipeline.py` → End-to-end QA pipeline
- `src/utils.py` → Helper functions

---

## ⚙️ Installation
Clone the repo:
```bash
git clone https://github.com/imtiazhumzah/DocuVision-QA.git
cd DocuVision-QA

---

💻 Usage
Run the notebook in Google Colab:
- Upload your PDF documents
- Build the indexes
- Ask natural language questions:
  query = "Summarize the methodology used in Table 2"
  answer = qa_pipeline.query(query)
  print(answer)

---

📊 Example Output

Query: "What does Figure 3 illustrate?"
Answer: "Figure 3 illustrates the architecture of the proposed deep learning model, showing the convolutional and pooling layers."
Citation: Page 12, Caption under Figure 3.

---

🔮 Roadmap
 Streamlit UI for interactive PDF QA
 Integration with LLaVA for stronger multimodal reasoning
 Deploy as API endpoint

---

🌟 Future Improvements
 - Add fine-tuned multimodal encoders for domain-specific PDFs
 - Deploy Streamlit / Gradio app for interactive use
 - Integrate graph-based retrieval for citations
 - Support multilingual documents

📧 Contact
👤 Imtiaz Ali
📩 Email: imtiazhumzah@gmail.com
🔗 LinkedIn: linkedin.com/in/imtiaz-ali-ab11162a5

