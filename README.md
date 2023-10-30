# Claims Q  

## Description  
The notebooks and code here may support efforts related to the 2023 GenAI Vendor Analysis effort.  

Enterprise effort to explore creating Generative AI solutions to business problems at USAA.  

The effort is organized into 5 use cases:  
1. Code-Assist  
2. HR-Assist  
3. Claims-Q  
4. Auto-Content  
5. MSR Co-Pilot  

The P&C Generative AI Use Case is as follows:  
Use Case: Medical record review and summarization for adjuster use  
Benefits: Improve claims accuracy  
Potential Solutions: Off-the-shelf LLM combined with in-context learning or fine-tuning  
Executive Sponsor: Larry Williams  
Available Tech:  
- Google – Vertex AI: Generative AI App Builder
- Microsoft – Open AI and Artificial Intelligence Suite
- IBM – IBM Watson product
USAA Labs Alpha environment to be used for development and testing


### LangChain Folder  
This folder contains notebooks that demonstrate how to interact with LLMs and Chatbots using the Langchain framework. 

- Different_Summarization_Types.ipynb - Demos how to execute the 4 various summarization types and includes commentary on which is best suited for which task.  Demos how to summarize a single text file and a webpage. Demos how to summarize an extremely large document such as a book.

- Hello_Local_LLMs.ipynb

- LangChain_Prompt_Templates.ipynb - Demonstrates different prompt templates and relevant formatting. Provides a detailed description of Langchain. Shows how to construct and run a HumanMessagePromptTemplate. This example relies on OPENAI_API_KEY.  

- LLM_Agent_React.ipynb - Demonstrates how to build a Langchain Agent. An agent consist of tools and the agent class type, which decides which actions to take. Tools are functions that agents can use to interact with the world. These tools can be generic utilities (e.g. search), other chains, or even other agents. This example relies on OPENAI_API_KEY. Output from LLM and Chat Models illustrate logical reasoning by the agent.  

- Question_a_Document.ipynb - Demonstrates how to construct a complete Langchain Question and Answer Flow. This includes Document Loading, Splitting, Storage using ChromaDB vector database, Retrieval, Prompt Templates and handling the response. Shows how to define a WebBaseLoader so you can ask a webpage some questions. Shows how to define ConversationBufferMemory to add memorry to a conversation.  

- Settlement_Demands.ipynb - loads a text file. the text file is info I manually scraped from a KDD webpage. LLM relies on a LLAMA2 model downloaded locally. Demonstrates multiple questions posed to the document. Demos custom prompt template. Demos adding memory to conversation and how to display memory object to output.

- Talk_to_DOI_Webpage.ipynb- Loads a TDI webpage. Uses Openai API key because this is a public webpage. Default model is gpt-3.5-turbo. Demo multiple questions posed to webpage. Demo text-davinci-003 with different temperature param values. Demos verbose logging to show reasoning steps.

- Talk_to_a_KDD_file.ipynb - Demonstrates how to load a split a text file. Define a QA chain using a Retriever and CharacterTextSplitter. Uses FAISS index vector store. Shows how to customize prompt templates and how to cite the source. Memory has been added to the conversational flow.  

- Talk_to_a_Medical_PDF.ipynb - Demos how to load a single PDF file and then ask questions. Demos how to summarize a text file. Demos different summarization types. Demos a prompt template and a refine template to refine the summarization output

- Talk_to_a_PDF.ipynb - This notebook is an implementation of Langchain Q&A chains. It demonstrates the ability for knowledge retrieval from a pdf document.  

- Talk_to_a_Webpage.ipynb - Demonstrates how to load a remote URL and perform knowledge retrieval using RetrievalQA.



## Authors
- Mark Lopez (PLB0171)
- Chris Haberland (PL0P539)



---

## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended steps.

## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin https://gitlab.rndalpha.com/chaberland/claims-q.git
git branch -M main
git push -uf origin main
```

## Integrate with your tools

- [ ] [Set up project integrations](https://gitlab.rndalpha.com/chaberland/claims-q/-/settings/integrations)

## Collaborate with your team

- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
- [ ] [Set auto-merge](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)


# langchain-work
