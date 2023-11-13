# AI-Enhanced Advertisement Generation

## Overview
This project demonstrates the use of Azure Cosmos DB for MongoDB vCore's vector similarity search and OpenAI embeddings to generate advertising content aimed at boosting sales. It is particularly tailored for a shoe retailer looking to leverage recent trends for effective advertising.

## Features
- **Vector Similarity Search**: Utilizes Azure Cosmos DB for MongoDB vCore to enhance semantic search capabilities within inventory data.
- **OpenAI Embeddings**: Leverages OpenAI embeddings to create vectors for inventory descriptions, enabling more nuanced matching with advertisement content.
- **Content Generation**: Generates catchy, trend-focused advertisements using OpenAI's language models.

## Prerequisites
- Azure OpenAI and Cosmos DB accounts.
- Necessary API keys and endpoints from Azure OpenAI and Cosmos DB services.
- Python environment (>= 3.9 version) with packages such as `numpy`, `openai`, `pymongo`, `python-dotenv`, `azure-core`, `azure-cosmos`, `tenacity`, and `gradio`.

## Setup and Configuration
1. **Azure OpenAI Setup**:
   - Follow the guide to create an Azure OpenAI resource. Access is granted by application at [Azure OpenAI Access](https://aka.ms/oai/access).
   - Deploy `completions` and `embeddings` models. Refer to the Azure OpenAI documentation for more details.
   - Note down your endpoint, key, and deployment names.

2. **Cosmos DB for MongoDB vCore Setup**:
   - Create a Cosmos DB resource following the guide provided in the Azure documentation.
   - Note down the connection details (server, user, pwd).

3. **Environment File**:
   - Use `example.env` as a template to fill in your keys and endpoints.
   - Rename the filled template to `.env` for the project to use.

## Running the Script
1. Install the required Python packages listed in the prerequisites.
2. Run the provided IPython notebook, which will guide you through the process of:
   - Loading and processing data.
   - Creating embeddings using Azure OpenAI.
   - Setting up and interacting with Cosmos DB.
   - Generating advertisements using OpenAI's language models.
   - Optionally, use `gradio` for creating an interactive web interface.

## Solution architecture
[solution architecture](./media/architecture.png)

## Output 
[Output screen](./media/Output.png)

## Usage
- The script can be modified to cater to different inventory types and advertisement themes.
- Experiment with different embeddings and models for varied content styles.

## Contributing
Contributions to this project are welcome. Please ensure to follow best coding practices and add relevant tests for new features.

## License

---
