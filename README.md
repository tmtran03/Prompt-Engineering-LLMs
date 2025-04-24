# GenAI for Software Development (Prompt Engineering for In-Context Learning)

* [1 Introduction](#1-introduction)  
* [2 Getting Started](#2-getting-started)  
  * [2.1 Preparations](#21-preparations)  
  * [2.2 Install Packages](#22-install-packages)  
  * [2.3 Run the fine-tuning model](#23-run-the-fine-tuning-model)  
* [3 Report](#3-report)  

---

# **1. Introduction**  
Prompt Engineering for In-Context Learning explores how different prompt designs influence Large Language Models (LLMs) in solving diverse software engineering tasks. In this assignment, we applied five strategies—zero-shot, few-shot, chain-of-thought, prompt-chaining, and BLEU-based self-consistency—to 22 problems ranging from code summarization and bug fixing to API generation and code translation. Our experiments compare two models—ChatGPT (gpt-4o-mini) and Codestral-2501—deployed on Azure, demonstrating how strategic prompt examples and structured reasoning affect code quality and clarity. Temperature is set to 0.7, and the token limit is 1024 for all tables.

The purpose of the code is to automate the generation of responses to our prewritten prompts.

---

# **2. Getting Started**  
This project is implemented in **Python 3.9+** and is compatible with **macOS, Linux, and Windows**.  

## **2.1 Preparations**  

(1) Clone the repository to your workspace:  
```shell
~ $ git clone https://github.com/tmtran03/Prompt-Engineering-LLMs
```
(2) Navigate into the repository:
```shell
~ $ cd Prompt-Engineering-LLMs
~/Prompt-Engineering-LLMs $
```
(3) Set up a virtual environment and activate it:
```
For macOS/Linux:
~/Prompt-Engineering-LLMs $ python -m venv ./venv/
~/Prompt-Engineering-LLMs $ source venv/bin/activate
(venv) ~/Prompt-Engineering-LLMs $ 
```

For Windows:
```shell
~/Prompt-Engineering-LLMs $ python -m venv .\venv\
~/Prompt-Engineering-LLMs $ .\venv\bin\Activate.ps1
(venv) ~/Prompt-Engineering-LLMs $
```
To deactivate the virtual environment, use the command:
```shell
(venv) $ deactivate
```

## **2.2 Install Packages**

Install the required dependencies:
```shell
(venv) ~/Prompt-Engineering-LLMs $ pip install -r requirements.txt
```

Make sure to have a token.txt with a personal GitHub token to run the AI models. 

## **2.3 Run the fine-tuning model**

(1) Run Fine-Tuning Demo

This script takes a list of problems that are already prompted by certain strategies and then runs each prompt based upon the models chosen. 
After the model is ran, then the script with the prompt, strategy uses, and output is all then logged in a csv that is created. 

Navigate to the ```src``` directory, then run:
```shell
(venv) ~/Prompt-Engineering-LLMs $ python src/genai_3.py
```

## 3. Report

The assignment report is available inside the ``reports`` folder named ``Assignment_Report.pdf``.
