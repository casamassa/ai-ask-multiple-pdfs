# AI - Case Study - Project Ask questions for multiple pdf documents

> You can find the tutorial for this project on [YouTube](https://youtu.be/dXxQ0LR-3Hg).

## Introduction

---

The MultiPDF Chat App is a Python application that allows you to chat with multiple PDF documents. You can ask questions about the PDFs using natural language, and the application will provide relevant responses based on the content of the documents. This app utilizes a language model to generate accurate answers to your queries. Please note that the app will only respond to questions related to the loaded PDFs.

## How It Works

---

![MultiPDF Chat App Diagram](./docs/PDF-LangChain.jpg)

The application follows these steps to provide responses to your questions:

1. PDF Loading: The app reads multiple PDF documents and extracts their text content.

2. Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

3. Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

## Dependencies and Installation

---

To install the MultiPDF Chat App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:

   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from HuggingFace and add it to the `.env` file in the project directory.

```commandline
HUGGINGFACEHUB_API_TOKEN=Your HuggingFaceHub API Token
```

To generate an API Token, create an account in HuggingFace website, then access https://huggingface.co/settings/tokens and create a token with write permission.

## Usage

---

To use the MultiPDF Chat App, follow these steps:

1. Ensure that you have installed the required dependencies and added the Hugging Face Hub key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:

   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions. Take care with the file size, as HuggingFace is free I could upload a small file to my tests.

5. Ask questions in natural language about the loaded PDFs using the chat interface.

## Contributing

---

This repository is intended for educational purposes and does not accept further contributions. It serves as supporting material for a YouTube tutorial that demonstrates how to build this project. Feel free to utilize and enhance the app based on your own requirements.

## License

---

The MultiPDF Chat App is released under the [MIT License](https://opensource.org/licenses/MIT).

## Notes

---

1. I choose use PyVenv to create virtual envorioment for my Python project, to ensure to use the Python version 3.9

First, make sure install Python 3.9 in your computer:

To install Python 3.9, run:

```
sudo apt update
sudo apt install python3.9
```

Make sure create your virtual envionment:

To create the virtual environment, run:

```
python3.9 -m venv name_of_virtual_env
```

For example: python3.9 -m venv venv

To activate your new virtual environment, run:

```
source name_of_virtual_env/bin/activate
```

For example: source venv/bin/activate

To deactivate your virtual environment, just run:
deactivate

## Requirements.txt commands

---

Install the required dependencies by running the following command:

```
pip install -r requirements.txt
```

Update all dependencies to last version by running the following command:

```
pip install --upgrade -r requirements.txt
```

If you install dependencies manually, to generate the file requirements.txt run the following command:
Para gerar o arquivo requirements.txt com as dependencias instaladas no ambiente virtual usar o comando:

```
pip freeze > requirements.txt
```

## References

---

https://instructor-embedding.github.io/
https://huggingface.co/hkunlp/instructor-xl
