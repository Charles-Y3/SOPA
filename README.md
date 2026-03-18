# SOPA (Smart Offline Personal Assistant) 
<p align="left">
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
  <img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" />
</p>

<p align="left">
  <img src="https://img.shields.io/badge/Privacy-100%25%20Offline-green?style=flat-square&logo=icloud&logoColor=white" />
</p>

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
   1. Chat Tab: Real-time interaction with the neural engine.
   2. Document Tab: Management and indexing of the local knowledge base.
   3. Translation Tab: Managing translation pairs ingested from documents or added manually.
   4. Chat History Tab: Persistent record of previous AI conversations for reference and retrieval.

D. Hardware-Aware Model Management

   SOPA automatically analyses available system resources and users may download and manage models locally through the integrated model manager.

E. Privacy

   SOPA is built to run entirely offline after user downloaded the LLM. 

F. Licensing

   SOPA (Smart Offline Personal Assistant) is distributed as free software for personal, educational, and research use. The software may be freely shared and redistributed in its original,      unmodified form.

   SOPA integrates open-source libraries including Python, ChromaDB, Whisper, CustomTkinter, NumPy, pandas, Matplotlib, and PyTorch. These components remain the property of their respective     authors and are used under their original licenses (e.g., MIT, BSD, Apache 2.0).

   SOPA does not distribute AI models. Users download compatible models (such as Qwen2.5 or Whisper models) directly from their original sources and must comply with the respective model       licenses.

G. Disclaimer

SOPA is an AI-assisted system designed to support human decision-making.
Important notes:
   1. SOPA is provided "as is" without warranty of any kind.
   2. AI-generated results may contain inaccuracies.
   3. Users are responsible for verifying outputs before use.
   4. The developers assume no liability for decisions made based on the software's outputs

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

# 🚀 Getting Started

To begin using SOPA, follow these initial steps:
* Navigate to Settings: Go to the Settings tab in the sidebar.
* Initial Setup: Click on Initial Setup to select the folder path containing the documents you wish to use for AI inference.
* Automatic Indexing: SOPA will read through the selected folders and ingest compatible files.

* Supported Formats: .pdf and .docx.
* Unsupported: Password-protected files and .doc formats will not be ingested.
* Auto-Translation: Translation vaults are automatically populated if double-column documents with different languages are detected.

# 🖥️ Main Interface
<p align="center"><img width="1384" alt="sopa1" src="https://github.com/user-attachments/assets/21a73cf2-08d7-4e25-9967-a5ec464e8ca0" /></p>

   * 💬 Chat: Engage in standard AI dialogue or ask specific questions about a file (e.g., abc.docx) already in your vault.
     
   * 🔍 Search: Perform a semantic search across your Document Vault. The system returns the top 3 matching segments with their original sources.
     
   * 🌐 Translate: Search the Translation Vault for existing phrases.
      * Matching results are returned with the source document quoted.Translate specific files.
      * If the segment already exists in the vault, SOPA retrieves it instead of re-translating.
        
   * 🤖 Auto: Automatically detects and directs your query to the most appropriate intent above.
     
   * 📤 Upload: Upload a single file for immediate use.
      * No Query: The file is added as Soft Memory (temporary and not retained after restart).
      * With Query: Directed automatically to the relevant intent.
      * Data Analysis: Uploading .xlsx or .csv allows for graph plotting and statistical analysis. Results are saved in the outputs folder.
      * Audio: Uploading .mp3 or .wav triggers transcription. Transcribed files are stored in the outputs folder.

# 📂 Tab Management
1. Document Vault

   * Filter: Use keyword search to quickly locate indexed documents.
   * Persistence: Convert files from Soft Memory to Hard Memory to ensure they are retained on system startup.
   * File Actions: Right-click to open a file, locate it in its folder, or delete it.
   * Preview: Double-click to view the content of a specific file.

2. Translation Vault

   * Management: Filter translation pairs by keyword or manually add, edit, and delete pairs.
   * View: Double-click to inspect a specific translation pair.

3. Chat History

   * Retrieval: Filter your previous conversations via keyword search.
   * Actions: Right-click to continue an old conversation or delete a record.
   * Review: Double-click to open and read a saved chat session.

4. Settings

   * Maintenance: Perform the initial setup or wipe all vault data.
   * Customization: Change the system language and toggle between Light and Dark modes.
      <p align="center"><img width="1159" alt="sopa3" src="https://github.com/user-attachments/assets/32835d51-98b6-4fca-8ba3-dc174416c336" /></p>
