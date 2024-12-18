# Explore Ollama

## Ollama

[Ollama](https://ollama.com) allows you to run Large Language Models (LLMs) locally on your machine, providing privacy and control over your AI interactions. This project serves as an example of how to integrate and work with [Ollama](https://ollama.com) in a locally hosted environment on macOS.

This project was developed and tested on the following:

- 2021 14" MacBook Pro
    - Apple M1 Max
    - 64GB RAM
    - 2TB SSD
    - macOS - `Sequoia 15.2`
    - Node.js - `v22.12.0`
    - npm - `v10.9.0`

## Installation

### Install Ollama

To install Ollama, follow these steps:

- Open a web browser and navigate to https://ollama.com/download
- Download the appropriate version for your operating system (macOS, Linux, Windows)
- On macOS, drag the downloaded file to the Applications folder
- Launch Ollama from the Applications folder and follow the instructions to complete the installation

Please see [Ollama](https://ollama.com/) for additional information.

## Run your first model

To view a list of available models installed on your machine, run the following command:

```bash
ollama list
```

This list will initially be empty. 🤓

To download, install and run your first model:

```bash
ollama run llama3.3
```

It will take a few minutes to download and install the model. This particular model is `42  GB` in size.

Once your model has downloaded, the [Llama 3.3 70B](https://ollama.com/library/llama3.3) model will be started and you will be able to interact with it in the terminal:

```bash
success 
>>> 
```

To see what commands are available, run the following command:

```bash
>>> /?
Available Commands:
  /set            Set session variables
  /show           Show model information
  /load <model>   Load a session or model
  /save <model>   Save your current session
  /clear          Clear session context
  /bye            Exit
  /?, /help       Help for a command
  /? shortcuts    Help for keyboard shortcuts

Use """ to begin a multi-line message.

```

## Remove or uninstall a model from your machine

If you would like to remove a model from your machine, you can do so by:

```bash
# List all models installed on your machine
ollama list
NAME               ID              SIZE     MODIFIED      
llama3.3:latest    a6eb4748fd29    42 GB    2 minutes ago    

# Remove a model from your machine
ollama remove llama3.3

# Verify the model has been removed
ollama list
NAME               ID              SIZE     MODIFIED      

```

## Download and install additional models

Please see [Models](https://ollama.com/search) to search, download, and install additional models on your machine.
