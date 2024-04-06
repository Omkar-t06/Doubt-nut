# Doubtnut

-----
## Introduction

Tired of staring endlessly at PDFs? Doubt-nut is your innovative solution! Ask questions directly to your PDFs in plain English, and get clear answers powered by AI. No more flipping through pages – Doubt-nut unlocks the knowledge within your notes, making learning active and efficient.

-----

## How it work?

![Doubt-Nut App Architecture](./docs/PDF-LangChain.jpg)

The application follows these steps to provide responses to your questions:

1. PDF Loading: The app reads multiple PDF documents and extracts their text content.

2. Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

3. Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

-----

## Dependencies and Installation

-----
To install the __Doubt-nut__, please follow these steps:

__Optional__ : Create a virtual environment. If you don't have idea about it please follow: [https://youtu.be/UPaN3Z49myw?si=rN4f9aHMVA4dZ1q-](https://youtu.be/UPaN3Z49myw?si=rN4f9aHMVA4dZ1q-)

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from [Gemini Ai Studio](https://aistudio.google.com/app/prompts/new_chat) and add it to the `.env` file in the project directory.
```commandline
GOOGLE_API_KEY = "YourAPIKeyShouldBeLikeThis"
```

__Note__ : You can also refer .env.example 

## Usage Guide
-----
To use the __Doubt-nut__, follow these steps:

1. Ensure that you have installed the required dependencies and added the OpenAI API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.
