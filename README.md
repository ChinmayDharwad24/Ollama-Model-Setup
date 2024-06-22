# Ollama Model Setup

This repository contains instructions and scripts for setting up and running Llama 3 and Gemma 2B models using Ollama on a Windows machine.

## Prerequisites

- [Ollama](https://ollama.com) installed on your Windows machine.

## Installation and Setup

### Step 1: Install Ollama

1. Download the Ollama installer for Windows from the [Ollama website](https://ollama.com/download).
2. Run the installer and follow the on-screen instructions.
3. Verify the installation by opening a browser and navigating to `http://localhost:11434`. You should see a message indicating that Ollama is running.

### Step 2: Download Models

Download the Llama 3 and Gemma 2B models using the following commands in Command Prompt:

- **Llama 3 8B:**
  ```sh
  ollama run llama3


# Gemma 2B Setup

This repository provides instructions and scripts for setting up and running the Gemma 2B model using Ollama on a Windows machine.

## Running Gemma 2B Model

To run the Gemma 2B model, follow these steps:

### Step 1: Install Ollama

Ensure that Ollama is installed on your Windows machine. If not, download the Ollama installer from the [Ollama website](https://ollama.com/download) and follow the installation instructions. Verify the installation by opening a browser and navigating to `http://localhost:11434`. You should see a confirmation message indicating that Ollama is running.

### Step 2: Download Gemma 2B Model

Download the Gemma 2B model using the following command in Command Prompt:

```sh
ollama run gemma:2b

## Starting Gemma 2B Model

To start the Gemma 2B model, use the provided script:

```sh
scripts\start_gemma2b.bat


## Interacting with Gemma 2B Model via API

You can interact with the Gemma 2B model using curl commands:

### Get a Response

```sh
curl http://localhost:11434/api/generate -d "{\"model\": \"gemma:2b\",\"prompt\":\"Why is the sky blue?\"}"


## Chat

```sh
curl http://localhost:11434/api/chat -d "{\"model\": \"gemma:2b\", \"messages\": [{ \"role\": \"user\", \"content\": \"why is the sky blue?\" }]}"


### File Descriptions

- `scripts/start_gemma2b.bat`: Batch script to start the Gemma 2B model.

### Troubleshooting

If you encounter any issues, please ensure that:

- Ollama is properly installed and running (http://localhost:11434 should be accessible).
- The Gemma 2B model is correctly downloaded and running.
- The curl commands are correctly formatted and executed.

For further assistance, refer to the Ollama documentation.