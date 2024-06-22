# Steps for downloading and running Llama3 and Llava:

## Steps for llama3
Step 1: Download Ollama
First, download the ollama tool from the official GitHub repository. You can find the repository here - https://github.com/ollama/ollama.

Step 2: Extract and Move Ollama
After downloading, extract the file and move the ollama executable to the Applications directory for easy access.

Step 3: Run Llama3 Model
Open your terminal and run the Llama3 model using the following command: ollama run llama3. This command starts the Llama3 model locally, making it available for interaction.

Step 4: Interact with Llama3 Model
Once the model is running successfully, you can interact with it using the curl command. Open a new terminal window and use the following command to ask the model a question:

curl -X POST http://localhost:11434/api/chat -H "Content-Type: application/json" -d '{
  "model": "llama3",
  "messages": [
    { "role": "user", "content": "what is Boston known for?" }
  ],
  "stream": false
}'

Usage
Running the Model: Use ollama run llama3 to start the Llama3 model.
Interacting with the Model: Use the provided curl command to send messages and receive responses from the model.

## Steps for llava
Step 1: Run Llava Model
Open your terminal and run the Llava model using the following command: ollama run llava. This command starts the Llava model locally, making it available for interaction.

Step 2: Interact with Llava Model
Once the model is running successfully, you can interact with it using the curl command. Open a new terminal window and use the following command to ask the model a question:

curl -X POST http://localhost:11434/api/chat -H "Content-Type: application/json" -d '{
  "model": "llava",
  "messages": [
    { "role": "user", "content": "what is Boston known for?" }
  ],
  "stream": false
}'
