# AI Documentation/Thesis Analystic BY LLM Model

### Introdctions
#### Business/ Use case 
We often obtain or download a lot of Document/Thesis from website internet.After that, we need spent a lot of the time to read multiple documents for understanding the context of these documents. It is taking a lot of time.

This project intended to be used LLM Model for the purpose of assisting the user to analyze and understand the context of these documents and faster access the context of the documents. 

### Technology use in this project
1. The first version will be used Google Gemini API for LLM Model , later versions will be try different open LLM models (e.g. LLama3, mi)

2. retrieval augmented generation (RAG) with langChain 
use for query the local Documentation
use LangChain to Question and Answer from local Documentation

3. Support Document
first version only pdf files format
later versions will be words, excel, may be also support image base documents

4. VectorDase
use Vector DataBase to store the converted Document context into embedding vector
use Vector Database can find document similarity 

5. FrontEnd UI
first version will be used Streamlit for Frontend UI
later versions will be Full stack with Backend Restful API


### Installation and Setup
1. use requirements.txt for installation package dependencies
2. you can setup virual environment by venv 
3. add your google api key to .env file  for enviroment variables 

### Run Application
1. Type command as below for running application
```
streamlit run apps.py 
```
2. Upload your document for query

3. Type chat prompt message to query the multiple documents