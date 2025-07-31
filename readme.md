# **Text Summarization & Named Entity Extraction**

You are given a collection of news articles (text). Your task is to build a system that can:
1.    Extract specific entities or key information from these documents (e.g., names, dates, locations, key metrics, sentiment, core issues).
2.    Generate concise summaries of the documents.
3.    Conceptual Agentic Component: Design how an AI agent could use this extraction and summarization capability as a "tool" to answer complex questions or perform specific tasks by navigating multiple documents.

## **Prerequisites**

Before you begin, ensure you have the following installed on your system:

* **Python 3.12:** This project requires Python version 3.12. You can download it from the [official Python website](https://www.python.org/downloads/).  
* **Git:** To clone this repository.

## **Installation**

Follow these steps to set up the project locally.

### **1\. Clone the Repository**

Open your terminal or command prompt and run the following command to clone the project repository:  
```
git clone https://github.com/your-username/your-repository-name.git  
cd your-repository-name
```

### **2\. Create a Virtual Environment**

It is highly recommended to use a virtual environment to manage project dependencies. This ensures that the packages you install for this project do not interfere with other projects.  
Run the following command to create a virtual environment named venv using Python 3.12.  
```
python3.12 \-m venv venv
```

**Note:** If python3.12 is not in your system's PATH, you may need to use the full path to the executable, or if you have Python 3.12 as your default, you can simply use python3.12 \-m venv venv.

### **3\. Activate the Virtual Environment**

Before installing dependencies, you must activate the virtual environment.

* **On macOS and Linux:**  
  ```
  source venv/bin/activate
  ```

* **On Windows:**  
  ```
  venv\\Scripts\\activate
  ```

You will know the environment is active when the terminal prompt changes to include (venv).

### **4\. Install Dependencies**

With the virtual environment active, install all the required packages listed in the requirements.txt file:  
```
pip install \-r requirements.txt
```

### **5\. Deactivating the Virtual Environment**

When you are finished working on the project, you can deactivate the virtual environment by simply typing:  
```
deactivate
```

## **Usage**
### **Create .env file**

Create a .env file in the same directory (your repo folder) with the following content. You must have your Azure OpenAI model Enpoint & keys in order to run the following section in the code notebook: Text Summarization (Abstractive) using LLM. Follow the documentation on Azure to know how to deploy your Azure OpenAI model instance if you already don't have one.
```
AZURE_OPENAI_ENDPOINT=<YOUR AZURE_OPENAI_ENDPOINT>
AZURE_OPENAI_API_KEY=<YOUR AZURE_OPENAI_API_KEY>
OPENAI_API_VERSION=<YOUR OPENAI_API_VERSION E.g.: 2024-12-01-preview>
```


Once the environment is set up and the dependencies are installed, you can run the code in the jupyter notebook by selecting the created venv as you kernel.  
\# Code Notebook

```
text-summarization-ner.ipynb
```
