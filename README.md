<div align="center">

# Hi, I'm Kambalapalle Kasi Reddy 👋

### AI/ML Engineer | GenAI | RAG | Computer Vision | Full-Stack

I build **production-oriented AI systems**, not just notebooks.

My work spans **LLM applications, RAG pipelines, machine learning, computer vision, APIs, and full-stack applications** — with a focus on turning real-world problems into working software.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/kambalapallekasireddy)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/kasireddy627)

</div>

---

## 👨‍💻 About Me

I'm a Computer Science graduate focused on **AI/ML Engineering and GenAI application development**.

I enjoy building systems where AI is only one part of the solution — combining **models, retrieval, APIs, databases, evaluation, deployment, and user interfaces** into a complete application.

### What I work on

* 🤖 **GenAI & RAG** — LLM applications, RAG pipelines, LangGraph, embeddings, vector databases
* 🧠 **Machine Learning** — classification, prediction, feature engineering, model evaluation, explainability
* 👁️ **Computer Vision** — object detection, OCR, image processing
* ⚙️ **Backend Engineering** — FastAPI, Flask, REST APIs, Docker
* 🌐 **Full-Stack Development** — React, Node.js, MongoDB, MySQL
* 🚀 **Deployment** — Docker, Streamlit, AWS

Currently building **Analyst-in-a-Box**, a FastAPI + LangGraph + FAISS based RAG application focused on turning documents into useful, grounded answers.

---

# 🚀 Featured Projects

## 01. 🤖 AI Podcast Generator

### Turning written content into podcast-style audio

**Problem**

People consume large amounts of news and long-form content but don't always have the time to read everything.

**What I built**

An end-to-end GenAI pipeline that transforms written articles into **podcast-style multilingual audio**.

### Engineering

* Extracted and processed article content
* Used LLMs to transform raw content into structured podcast-style scripts
* Generated natural-language audio using neural TTS
* Built APIs using **FastAPI**
* Created an interactive interface using **Streamlit**
* Containerized the application using **Docker**
* Designed the pipeline so individual stages can be modified independently

### Tech Stack

`Python` `LLM` `Groq` `FastAPI` `Streamlit` `Docker` `TTS`

### Why this project matters

This isn't simply an LLM wrapper.

It demonstrates the ability to build an **end-to-end AI application** involving:

`Input → Processing → LLM → Structured Output → TTS → Audio → Application`

🔗 **[View Repository](https://github.com/kasireddy627/AI_PODCAST_GENERATOR)**

---

## 02. 📚 RAG Chatbot — Appening Infotech Interview Task

### Building a grounded question-answering system

**Problem**

General-purpose LLMs can generate convincing answers that aren't supported by the source material.

For knowledge-base applications, the system needs to retrieve relevant information before generating an answer.

**What I built**

A **RAG-based chatbot** that answers questions strictly from an Agentic AI knowledge base.

### Architecture

```text
PDF
 ↓
Document Loading
 ↓
Text Chunking
 ↓
Embeddings
 ↓
Pinecone Vector Database
 ↓
Similarity Retrieval
 ↓
LangGraph Workflow
 ↓
Gemini LLM
 ↓
Grounded Answer
```

### Engineering

* Processed the source PDF into searchable chunks
* Generated vector embeddings for semantic retrieval
* Stored embeddings in **Pinecone**
* Implemented retrieval using similarity search
* Built the workflow using **LangGraph**
* Used **Gemini** for answer generation
* Designed prompts to keep responses grounded in retrieved context
* Returned retrieved chunks and similarity scores alongside the answer
* Exposed the application through **FastAPI**
* Built a lightweight **Streamlit** interface for testing

### Tech Stack

`Python` `LangGraph` `LangChain` `Gemini` `Pinecone` `FastAPI` `Streamlit`

### Key Engineering Focus

The important part of this project wasn't simply calling an LLM.

It was designing the complete pipeline:

**Retrieval → Context → Generation → Grounding**

🔗 **[View Repository](https://github.com/kasireddy627/Appening-Infotech-AI-Engineer---Interview-Task)**

---

## 03. 📊 Customer Retention Intelligence

### Predicting customer churn before revenue is lost

**Problem**

Businesses often identify customer churn only after the customer has already left.

The goal was to predict customers who are likely to churn and provide an interpretable prediction that can support retention decisions.

**What I built**

A machine-learning application that predicts customer churn and explains **why the model made its prediction**.

### Engineering

* Performed data preprocessing and feature analysis
* Trained and evaluated multiple ML approaches
* Used **XGBoost** for churn prediction
* Tuned the decision threshold instead of blindly using `0.50`
* Used **SHAP** to explain individual predictions
* Built an interactive Streamlit dashboard
* Exposed model predictions in a user-friendly format

### Tech Stack

`Python` `XGBoost` `Scikit-learn` `SHAP` `Pandas` `Streamlit`

### Why the threshold matters

A churn model isn't useful simply because it has high accuracy.

For a retention problem, the cost of:

**False Negative → Missed customer at risk**

can be very different from:

**False Positive → Unnecessary retention action**

The project therefore treats the classification threshold as a business decision rather than an arbitrary default.

🔗 **[View Repository](https://github.com/kasireddy627/Customer-Retention-Intelligence-ML_Model)**

---

## 04. 🚗 Automatic License Plate Recognition

### Detecting and reading vehicle license plates

**Problem**

Manually identifying license plates from vehicle images is slow and difficult to scale.

**What I built**

An end-to-end **Automatic License Plate Recognition system** that detects license plates and extracts their text from uploaded vehicle images.

### Pipeline

```text
Vehicle Image
      ↓
YOLOv8 License Plate Detection
      ↓
License Plate Crop
      ↓
Image Processing
      ↓
EasyOCR
      ↓
Detected Plate Number
```

### Engineering

* Trained a custom **YOLOv8** license plate detector
* Processed vehicle images using **OpenCV**
* Cropped detected license plate regions
* Applied OCR using **EasyOCR**
* Added inference-time measurements for:

  * Detection
  * OCR
  * Total processing time
* Built a Streamlit interface
* Displayed the original image, detected plate crop, prediction, and performance metrics

### Example Performance

```text
Detection Time : ~68 ms
OCR Time       : ~130 ms
Total Time     : ~198 ms
```

### Tech Stack

`Python` `YOLOv8` `OpenCV` `EasyOCR` `Streamlit`

🔗 **[View Repository](https://github.com/kasireddy627/CNN-CV-PROJECT-ALPR_NUMBER_PLATE_DETECTION)**

---

# 🧠 Currently Building

## Analyst-in-a-Box

A document intelligence system designed around **RAG + LangGraph + FastAPI + FAISS**.

The objective is to move beyond a basic chatbot and build a system that can:

* Ingest business documents
* Retrieve relevant information
* Reason over retrieved context
* Generate grounded answers
* Expose functionality through APIs
* Provide a usable application layer

**Core Stack**

`Python` `FastAPI` `LangGraph` `FAISS` `LLMs` `RAG`

---

# 🛠️ Technical Skills

### AI / Machine Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square\&logo=python\&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square\&logo=pytorch\&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square\&logo=scikitlearn\&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square\&logo=opencv\&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square\&logo=pandas\&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square\&logo=numpy\&logoColor=white)

### GenAI / LLM Engineering

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square\&logo=langchain\&logoColor=white)

`RAG` `LangGraph` `LLM Applications` `Embeddings` `Vector Databases` `Prompt Engineering` `Agentic AI`

### Backend / Deployment

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square\&logo=fastapi\&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square\&logo=flask\&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square\&logo=streamlit\&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square\&logo=docker\&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square\&logo=amazonaws\&logoColor=white)

### Full-Stack / Databases

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square\&logo=react\&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square\&logo=nodedotjs\&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square\&logo=mongodb\&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square\&logo=mysql\&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square\&logo=git\&logoColor=white)

---

# 📌 Other Projects

More projects are available in my repositories, including:

* Sentiment Analysis
* Customer Segmentation
* SQL Analytics
* Full-Stack LMS
* Machine Learning Applications
* Computer Vision Applications
* React UI Projects

🔗 **[Explore All Repositories](https://github.com/kasireddy627?tab=repositories)**

---

# 📈 GitHub Activity

<div align="center">

![Kasi's GitHub Stats](https://github-readme-stats.vercel.app/api?username=kasireddy627\&show_icons=true\&theme=default\&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=kasireddy627\&layout=compact\&hide_border=true)

</div>

---

# 🎯 What I'm Looking For

I'm looking for opportunities where I can contribute as an:

**AI/ML Engineer · GenAI Engineer · Data Scientist · Software Engineer**

I'm particularly interested in teams building:

* LLM-powered products
* RAG and knowledge systems
* AI automation
* Machine-learning applications
* Computer vision systems
* Data-driven products

📍 Hyderabad, India · Open to remote opportunities

---

<div align="center">

### Let's build something useful with AI.

[![LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/kambalapallekasireddy)

</div>
