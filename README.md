# Content Generation and Validation in Digital Marketing

## Overview

This project focuses on generating and validating digital marketing content that aligns with a company's guidelines and tone of voice using large language and multimodal models. This version of the marketing demo has been adjusted for Azure OpenAI services.

## Setup

Follow the steps below carefully to set up your environment.

### Prerequisites

#### 1. Create a Python Virtual Environment

You can create a virtual environment using `python venv`, `conda`, or your preferred method.

```shell
# Create a virtual environment
python -m venv folderName

# Activate the virtual environment
folderName\Scripts\activate  # Windows
source folderName/bin/activate  # macOS/Linux
```

#### 2. Install Jupyter Lab

Once the virtual environment is activated, install Jupyter Lab. While the installation is running, create the `.env` file.

```shell
pip install jupyterlab
```

#### 3. Configure the `.env` File

Create a `.env` file and add the following configuration:

```shell
# GENERAL CONFIG
AZURE_ENDPOINT = "your_endpoint_here"
AZURE_OPENAI_API_KEY = "your_api_key_here"

# Embedding Model Configuration
EMBEDDING_MODEL = "text-embedding-3-small"
EMBEDDING_VERSION = "2024-02-01"
EMBEDDING_DEPLOYMENT = "embedding"

# Chat Model Configuration
CHAT_MODEL = "gpt-4"
CHAT_VERSION = "2024-02-15-preview"
CHAT_DEPLOYMENT = "demo-chat-gpt4"
```

With the prerequisites complete, proceed to initialization.

## Initialization

1. Open Jupyter Lab and run the first cell to install the required dependencies:

```shell
jupyter lab
```

2. After running the initial cell, execute the pipeline cell.
3. Close Jupyter Lab to finalize the installation.

## Running the Program

To run the program, use the following command and open the provided URL:

```shell
streamlit run streamlit_app_new_experiment1.py
```

## Troubleshooting guide:

### If app doenst work?

Check the steps bellow:

- Check your env variables
- Check the api version for deprication
- Test the model through a new cell in jupyterlab
