# LexiQ – Legal Question Answering System

LexiQ is a domain-specific Legal QA system designed to help lawyers, researchers, and students query legal documents (PDFs) directly with structured, context-aware answers.

---

## 🔍 Key Features

- **📂 Multi-PDF Legal QA:** Upload and query multiple legal PDFs at once.
- **🧠 Custom Legal Model:** Fine-tuned Mistral-7B using [CUAD](https://huggingface.co/datasets/lexpredict/legal-contract-qa) and [SARA](https://huggingface.co/datasets/jhu-clsp/SARA) datasets with LoRA + 4-bit quantization for efficiency.
- **🔎 RAG Pipeline:** Retrieval-Augmented Generation using LangChain and FAISS for pinpointing relevant legal context.
- **⚡ Productivity Focused:** Drastically cuts down manual reading time for legal research, contracts, and compliance documents.

---

## 📁 Project Structure

```

LexiQ/
├── notebooks/
│   ├── major-law-new-model.ipynb             # Fine-tuning Mistral-7B
│   ├── major-multi-law-pdf-reader.ipynb      # QA over multiple PDFs
│   └── major-single-law-pdf-reader.ipynb     # QA over a single PDF
│
├── data/
│   └── CUADv1.json                           # CUAD dataset (for demo only)
│
├── examples/
│   ├── Case File.pdf
│   └── Department of Justice Brief.pdf
│
├── requirements.txt
└── README.md

````

> ⚠️ **Note**: CUAD dataset is included for demonstration only. The SARA dataset can be accessed [here](https://huggingface.co/datasets/jhu-clsp/SARA).

---

## 🧠 Model & Datasets

| Component     | Description |
|---------------|-------------|
| **Base Model** | Mistral-7B |
| **Fine-tuning** | LoRA + 4-bit Quantization |
| **Datasets** | [CUAD](https://huggingface.co/datasets/lexpredict/legal-contract-qa) (Contract Understanding), [SARA](https://huggingface.co/datasets/jhu-clsp/SARA) (Structured Abstractive Reading) |

