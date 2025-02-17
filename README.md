# D2COpenAIPlugin

> **Join the [ChatGPT plugins waitlist here](https://openai.com/waitlist/plugins)!**
> 
> [my GTPs with the plugin](https://chat.openai.com/g/g-B1Bfoq5qh-uml-diagram-creation-expert)

D2COpenAIPlugin is a plugin for ChatGPT that enables users to generate diagrams using PlantUML or Mermaid. This plugin enhances the capabilities of ChatGPT by providing a seamless way to create diverse and creative diagrams.

![https://github.com/antoinebou12/UMLOpenAIPlugin/docs/DiagramGeneratorPlugin.gif](https://raw.githubusercontent.com/antoinebou12/UMLOpenAIPlugin/main/docs/DiagramGeneratorPlugin.gif)
![image](https://github.com/antoinebou12/D2COpenAIPlugin/assets/13888068/638e6ef6-b006-4f63-a7b8-b765fc0d8a41)

## Features
- Generate diagrams using PlantUML or Mermaid
- Seamless integration with ChatGPT
- User-friendly interface for creating diagrams
- Enhances the versatility of ChatGPT

## Installation
Before using the plugin, make sure to have the following prerequisites installed:

- Python 3.6+
- FastAPI
- uvicorn

1. Install Python 3.10, if not already installed.
2. Clone the repository: `git clone https://github.com/antoinebou12/D2COpenAIPlugin.git`
3. Navigate to the cloned repository directory: `cd /path/to/D2COpenAIPlugin`
4. Install poetry: `pip install poetry`
5. Create a new virtual environment with Python 3.10: `poetry env use python3.10`
6. Activate the virtual environment: `poetry shell`
7. Install app dependencies: `poetry install`
8. Create a [bearer token](#general-environment-variables)
9. Set the required environment variables:

## Setup

To install the required packages for this plugin, run the following command:

```bash
pip install -r requirements-dev.txt
```

To run the plugin, enter the following command:

```bash
python app.py
```

Once the local server is running:

```bash
uvicorn app:app --host 127.0.0.1 --port 5003
```

1. Navigate to https://chat.openai.com.
2. In the Model drop down, select "Plugins" (note, if you don't see it there, you don't have access yet).
3. Select "Plugin store"
4. Select "Develop your own plugin"
5. Enter in `localhost:5003` since this is the URL the server is running on locally, then select "Find manifest file".

The plugin should now be installed and enabled! You can start with a question like "What is on my todo list" and then try adding something to it as well!


### Testing in ChatGPT

To test a locally hosted plugin in ChatGPT, follow these steps:

1. Run the API on localhost: `poetry run dev`
2. Follow the instructions in the [Testing a Localhost Plugin in ChatGPT](#testing-a-localhost-plugin-in-chatgpt) section of the README.

For more detailed information on setting up, developing, and deploying the ChatGPT Retrieval Plugin, refer to the full Development section below.


## Getting help

If you run into issues or have questions building a plugin, please join our [Developer community forum](https://community.openai.com/c/chat-plugins/20).
