# Ollama Chatbot

This Python script creates a chatbot interface using the Gradio library.

## Dependencies
- requests: Used for making HTTP requests.
- json: Used for handling JSON data.
- gradio: Used for creating the chatbot interface.

## How it works
The script sets up a Gradio interface for a chatbot. The chatbot communicates with an API endpoint (in this case, "http://localhost:11434/api/generate") to generate responses.

When a user enters a prompt, the script appends it to the conversation history and sends a POST request to the API with the entire conversation history as the prompt. The API is expected to return a response which is then added to the conversation history and displayed to the user.

If the API returns a status code other than 200, the script prints an error message.

## Usage
To run the chatbot, simply execute the script. A Gradio interface will launch, where you can enter your prompts and see the chatbot's responses.

Command to run the script:

python ollamaChatbot.py