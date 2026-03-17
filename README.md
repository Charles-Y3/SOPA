# SOPA (Smart Offline Personal Assistant) 

SOPA (Smart Offline Personal Assistant) is a specialised local AI platform designed for secure, high-precision document intelligence and data analysis. SOPA operates entirely offline, ensuring data privacy. The system integrates Large Language Models (LLMs), vector databases, and a Retrieval-Augmented Generation (RAG) pipeline to enable advanced document search, translation, and analytical capabilities within a unified local workspace.

A. Core Features
   1.	Multiformat Ingestion such as pdf, docx, txt, csv, xlsx, mp3 and wav
   2.	Semantic Search (RAG-Powered) which uses vector databases (ChromaDB) to perform contextual search across stored documents
   3.	Audio Transcription: converts audio files into searchable text documents
   4.	A dedicated translation pipeline that validates using semantic similarity scoring and allows translation generation based on stored translation pairs
   5.	Statistical analysis and graph generation

B. Intelligent Task Routing
   1.	Auto task routing: SOPA analyses the user query and determines the appropriate processing engine.
   2.	User-Specified Intent: Users can also manually specify the task type if precise control is required.

C. Modular Design
The interface features a tab-based navigation system:
   •	Chat Tab: Real-time interaction with the neural engine.
   •	Document Tab: Management and indexing of the local knowledge base.
   •	Translation Tab: Managing translation pairs ingested from documents or added manually.
   •	Chat History Tab: Persistent record of previous AI conversations for reference and retrieval.

D. Hardware-Aware Model Management
SOPA automatically analyses available system resources and users may download and manage models locally through the integrated model manager.

E. Privacy
SOPA is built to run entirely offline after user downloaded the LLM. 

F. Licensing
SOPA (Smart Offline Personal Assistant) is distributed as free software for personal, educational, and research use. The software may be freely shared and redistributed in its original, unmodified form.

SOPA integrates open-source libraries including Python, ChromaDB, Whisper, CustomTkinter, NumPy, pandas, Matplotlib, and PyTorch. These components remain the property of their respective authors and are used under their original licenses (e.g., MIT, BSD, Apache 2.0).

SOPA does not distribute AI models. Users download compatible models (such as Qwen2.5 or Whisper models) directly from their original sources and must comply with the respective model licenses.

G. Disclaimer
SOPA is an AI-assisted system designed to support human decision-making.
Important notes:
   •	SOPA is provided "as is" without warranty of any kind.
   •	AI-generated results may contain inaccuracies.
   •	Users are responsible for verifying outputs before use.
   •	The developers assume no liability for decisions made based on the software's outputs

