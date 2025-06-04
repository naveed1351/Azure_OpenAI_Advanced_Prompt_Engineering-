# Azure_OpenAI_Advanced_Prompt_Engineering
 

Repository Overview:
 
This repository is dedicated to writing, optimizing, and engineering prompts for Azure OpenAI's latest language models. It covers best practices and advanced techniques for prompt engineering, as highlighted in the OpenAI Prompt Engineering Guide and supports the latest models, including GPT-4.1, GPT-4o, and other deployed versions. Use these materials to learn, experiment, and excel in prompt design for generative AI applications on Azure.
 

Pre-requisites:
 

- Azure ML Workspace
- Compute Instance per attendee
- Azure OpenAI (AOAI) Resource with required models deployed
- Bing Resource
- Note: Bing Search will be retired in August 2025. Plan for alternative services.
 

Deployment Steps as below:
 

1. Deploy Required AOAI Models:
 

In Azure AI Foundry /OpenAI → Deployments, ensure the following models are deployed (in the Sweden Central Region, or your relevant region):
- gpt-4o 
- gpt-4.1
- Note the deployment names; you’ll need them in the notebooks.
 

2. Set Up Your Environment:
 

- Open Azure Machine Learning Studio
- Go to Notebooks
- Start your Compute Instance
- Open the Terminal
 

3. Clone the Repository:
 
git clone https://github.com/naveed1351/Azure_OpenAI_Advanced_Prompt_Engineering-.git
cd AzureOpenAI_Advanced_Prompt_Engineering  
 

4. Prepare Python Environment:
 
- Use Python 3.10 (recommended with Conda):

- conda activate azureml_py310_sdkv2  


5. Install Dependencies:
 

- pip install -r ./common/requirements.txt  
 
- Ensure you install dependencies in the same environment you’ll use for the notebooks.
 

6. Configure Credentials: Edit the credentials.env file with your values:

- AZURE_OPENAI_ENDPOINT
- AZURE_OPENAI_API_KEY

- AZURE_OPENAI_CHAT_ENDPOINT
- AZURE_OPENAI_CHAT_KEY

- MANAGED_IDENTITY_CLIENT_ID

(Find these in Azure Portal → Azure OpenAI Resource → Keys and Endpoint.) For Specific Chat model, you can find the endpoint and keys in the AI Foundry.
 

7. (Optional) Create Bing Resource: Note: Bing Search will be retired August 2025.


Go to Azure Portal → Bing Resources → Add ‘Bing Search’ → Review and Create
Add BING_SUBSCRIPTION_KEY & BING_SEARCH_URL to your credentials.env file.
 

Notebooks Overview:
 

Notebook 07.0 & 07.1: Advanced prompt engineering with GPT-4o and GPT-4.1
Other notebooks: Prompt evaluation, function calling, OpenAI usage tracking, and best practices.


This repo follows prompt engineering best practices as described by OpenAI, providing hands-on materials to improve your prompt design and performance with Azure OpenAI models.

 
For questions or issues, see the documentation.