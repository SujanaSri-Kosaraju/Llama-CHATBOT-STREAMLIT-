# Custom Chatbot Creation for PDF data Retrieval.

## Overview

The goal of this project is to create a user-centric and intelligent system that retrieves the information from PDF documents through natural language queries. The project focuses on developing an interface, allowing users to interact with PDF content using language that they are comfortable with.


### Requirements

1. Input: Give any pdf document as an input(can be multiple aswell).
2. VectoreStore: The pdf's are then converted to vectorstore using FAISS vector database and llama-2-7b-chat.ggml Embeddings model from Hugging Face.
3. Memory: Conversation buffer memory is used to maintain a track of previous conversation which are fed to the llm model along with the user query.(history)
4. Text Generation: The embedded input is fed to the model with Llama's replicate api key.
5. User Interface: Streamlit is used to create the interface for the application.

###Streamlit:
	Streamlit is just a framework like Flask, which is used to provide interface for the application.


### Why llama-2-7b-chat.ggmlv3 model??

- This is a sentence transormation model, which is trained on large datasets to understand the relation between different sentences/words, which helps in generating accurate outputs.
- This is a pretrained model.


###To use PDF data Retrieval chatbot:

1. Install dependencies:
  	
	 pip install -r requirements.txt
  

2. Run the streamlit application:

   	streamlit run app.py


3. Open the browser and navigate to the local host to access the user interface.

4. Enter the question related to the document.



###Deployment of the app:

1.Go to share streamlit (https://share.streamlit.io/) in your browser.

2.click "New app" which is on the upper-right corner.

3.Go to paste Github URL and paste the "app.py" path directly from github(____________app.py)

4.Click on Deploy.
