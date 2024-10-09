# Create a ChatGPT For Your PDF in Python and Langchain

This is a Python application that allows you to load a PDF and ask questions about it using natural language. The application uses a LLM to generate a response about your PDF. The LLM will not answer questions unrelated to the document.

# How it works

The application reads the PDF and splits the text into smaller chunks that can be then fed into a LLM. It uses OpenAI embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.

The application uses Streamlit to create the GUI and Langchain to deal with the LLM.

# Installation

To install the repository, please clone this repository and install the requirements:

```
pip install -r requirements.txt
```


You will also need to add your OpenAI API key to the .env file.

# Usage

To use the application, run the main.py file with the streamlit CLI (after having installed streamlit):

```
streamlit run app.py
```

Result:

<img width="608" alt="Screenshot 2024-03-08 at 20 52 01" src="https://github.com/redjules/Create-a-ChatGPT-For-Your-PDF-in-Python-and-Langchain/assets/106017493/8b32e0ce-d1cd-4167-b070-8eca434a80b1">

![Screenshot 2024-03-08 at 20 59 45](https://github.com/redjules/Create-a-ChatGPT-For-Your-PDF-in-Python-and-Langchain/assets/106017493/0689e157-a175-4843-96af-993a4b4b2e0e)


![Screenshot 2024-03-08 at 21 00 38](https://github.com/redjules/Create-a-ChatGPT-For-Your-PDF-in-Python-and-Langchain/assets/106017493/d761be15-f505-46fc-913c-3a41c8f9b224)


We also track how much money we are spending per question:


<img width="332" alt="Screenshot 2024-03-08 at 20 53 33" src="https://github.com/redjules/Create-a-ChatGPT-For-Your-PDF-in-Python-and-Langchain/assets/106017493/942ca062-a41b-4f51-b016-98bc7847f491">


