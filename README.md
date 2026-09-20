<h1 align="center">🧑‍⚖️ ParlaMentis: AI for the Italian Chamber of Deputies</h1>

> **Note:** The source code for this project is closed-source and property of UniboNLP / DISI (University of Bologna) due to institutional agreements. This repository serves as a technical overview of my Bachelor's Thesis contributions. You can read the full technical documentation in the uploaded thesis: [Tesi di Laurea Triennale - Giorgio Fantilli.pdf](./Tesi_di_Laurea_Triennale_Giorgio_Fantilli.pdf).

## 📌 Project Overview
Developed in response to an official call from the Italian Chamber of Deputies, ParlaMentis is a multi-language, multi-task conversational agent. It is designed to assist Italian parliamentarians in drafting legislative acts by providing guided comprehension, semantic access to multi-modal sources, and updated regulatory context.

## 🛠️ My Technical Contributions
During this experimental thesis project under the supervision of Prof. Gianluca Moro, I actively contributed to the end-to-end development of the system:

*   **Data Engineering & Web Scraping:** Built automated Python pipelines using `SPARQL`, `PDFMiner`, and `Selenium` to extract and structure data from the Chamber's Linked Open Data (OCD) and WebTV portal. This included parsing complex two-column legal PDFs and extracting video intervention transcripts.
*   **AI Architecture (Multi-Document Agent):** Implemented an advanced Retrieval-Augmented Generation (RAG) system integrated with the ReAct (Reasoning and Acting) paradigm using `LlamaIndex`. The architecture utilizes a Top-Level Agent for query planning and multiple Document Agents for specific retrieval tasks.
*   **LLM Fine-Tuning:** Handled the instruction fine-tuning of `Meta-LLaMA-3-8B`. Applied Continual Pre-Training (CPT) and Odds Ratio Preference Optimization (ORPO) to adapt the model to the Italian legal domain and format.
*   **Frontend Development:** Developed a React.js chatbot interface to allow users to easily interact with the agent and manually review the retrieved legal sources (PDFs and video clips).

## ⚙️ Core Technologies
*   **AI & ML:** Python, HuggingFace, LlamaIndex, Meta-LLaMA-3-8B
*   **Data Extraction:** SPARQL, Selenium, PDFMiner
*   **Frontend:** React.js, JSX
