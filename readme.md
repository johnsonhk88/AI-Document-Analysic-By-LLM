# AI Documentation/Analystic BY LLM Model (Multimodal)

### Introdctions
#### Business/ Use case 
We often obtain or download a lot of Document from website internet.After that, we need spent a lot of the time to read multiple documents for understanding the context of these documents. It is taking a lot of time.

This project intended to be used LLM Model for the purpose of assisting the user to analyze and understand the context of these documents and faster access the context of the documents. 

This project can divide into 3 parts
1. Document Data Extraction Algorithms
2. Data Analysis Algorithms for Documentation
3. Data Retrieval Algorithms for Documentation (RAG+ LLM Model)

### Technology use in this project
1. Document Data Extraction (Unstructure Document Preprocssing)
- Because the input document complexity, include table, image (chart), I will use several AI model  like OCR , commputer vision model, Vision transformer , layout transformer, Embedding model to extract and analysis the document content from bank statement.
- Complex layout/Context format Analysis by ML model
- use advance rule base model or Machine learning  model :
  - group and reorganize the data into a user-friendly format. (no experience to build rule to graoup data)
  - Identify common denominators and create headers for each group. (no experence)
  - Display only the differences between similar items (e.g., window sizes, owners) as line items below each header. 
  - Automate the process using AI, enabling the system to self-learn and understand the data structure.  
  - Extract relevant data from PDFs with different layouts and formats.

2. Document Analysis
- Classification the document type 
- Documentation content summary
- Intelligence Extract Data and output structure data


3. Vector DataBase
use Vector DataBase to store the converted Document context into embedding vector
use Vector Database can find document similarity 

4. Retrieval augmented generation (RAG) with Multimodal 
use for query the local Documentation
use LangChain to Question and Answer from local Documentation



5. The first version will be used Google Gemini API for LLM Model , later versions will be try different open LLM models (e.g. LLama3, mi)


6. Support Document
first version only pdf files format
later versions will be words, excel, may be also support image base documents

7. FrontEnd UI
first version will be used Streamlit for Frontend UI
later versions will be Full stack with Backend Restful API


### Installation and Setup
1. use requirements.txt for installation package dependencies
2. you can setup virual environment by venv 
3. add your google api key to .env file  for enviroment variables 

### Run Application
1. run development version : go to "dev" folder

2. run demo version: go to "demo" folder
- Type command as below for running application
```
streamlit run apps.py 
```
- Upload your document for query

- Type chat prompt message to query the multiple documents
