# SOPA Smart Offline Personal Assistant 

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

***********************************************************************************************************************************************************************************************

Getting Started

To begin, navigate to the Settings tab and select Initial Setup to provide SOPA with the folder path that contains the documents it will use for inference. It will read inside folders and works for .docx and .pdf documents. Password protected and .doc documents will not be ingested into the vaults. Translation vaults are automatically populated for double column documents with different languages.

Main Interface
 

What you can do
1.	Specify the intent:
 
a.	Chat: to chat with the AI
i.	Normal chat
ii.	Ask queries about a filename with the extension (e.g. abc.docx that is in the document vault)

b.	Search: looks through your document vault using semantic search
i.	Return at most the top 3 matched document segments with their sources

c.	Translate: looks through the translation vault using semantic search
i.	Translate any phrase to other languages. If matching translation exist in the translation vault, it will be returned with the source document quoted.
ii.	Translate a filename with the extension (e.g. abc.docx that is in the document vault) to another language. If segments exist in the translation vault, it will be used instead of translating it again.

d.	Auto: automatically direct your query to one of the intents above

e.	Upload: allows one file to be uploaded. 
i.	If no query is given, it will be added to the document vault with memory type as soft (soft type memory are not retained on startup).
ii.	Otherwise, it will automatically be directed to one of the intents.
iii.	If .xlsx or .csv files are uploaded, you can ask it to plot graphs and perform statistical analysis. Graphs can be found in the ‘outputs’ folder.
iv.	If .mp3 or .wav files are uploaded, it will be transcribed and link to the transcription will be given. The transcribed file can be found in the ‘outputs’ folder.

2.	In the tab: Document Vault, you can
a.	Use keyword search to filter the documents
b.	Convert files from soft type memory to hard type (hard type memory are retained on startup)
c.	Right click to open file, go to the folder or delete that file
d.	Double-click to look at the content of a particular file

3.	In the tab: Translation Vault, you can
a.	Use keyword search to filter the translation pairs
b.	Add, edit or delete any translation pairs
c.	Double-click to look at the translation pairs

4.	In the tab: Translation Vault, you can
a.	Use keyword search to filter the chat history
b.	Right click to continue or delete a chat
c.	Double-click to look at a particular saved chat 

5.	In the tab: Settings, you can
a.	Do initial setup or to delete all the data in the vaults
b.	Change the language and mode (light or dark)
 




