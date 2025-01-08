# tds_capstone
Capstone Project for 'Topics in Data Science' 

Project executed by **Alexander Keßler** and **Dominik Schuster**

### To dos for next time
* Generating a QA-dataset with Gemini -> one sentence as answer (Alex)
* Generating a QA-dataset vie Huggingface -> one sentence as answer (Domi)

##### How the dataset should look like
* Multiple (5) contexts per possible combination of answers -> transfer multiple choice into single choice
* contains entries of Q + context + answer (for multiple choice, convert "old" answer options into new one)
* At first, concentrate on single/multiple choice

### The task
The task is described in the following:

* Deadline for documentation & materials: 02.02.2025
* Presentation date: 03.02.2025

In this project, you are tasked to generate your Question & Answering (QA) dataset based on the structure of the questionnaires from snapADDY, which you can find in this section. Then, you will develop strategies to evaluate your dataset using pre-trained Q&A models, potentially from HuggingFace. 

#### **Main Tasks:**

1. Generate a Q&A dataset by creating text descriptions for the questionnaires provided by snapADDY. It would help if you incorporated several prompt engineering techniques to design good prompts for generating the texts. Some ideas to start:
* Use chatGPT or similar chatbots to generate texts based on the questionnaires
* Use pre-trained models on HuggingFace programmatically, i.e., calling APIs to generate responses
  * Classic deep learning models: RoBERTa, DistilLBert, etc.
  * Popular large language models (LLMs): LLaMa-based models, Gemini (Flash 1.5), etc
* Advanced: create a small dataset based on one of the methods above, then fine-tune a model on this dataset to generate similar pairs to create more samples
* You are welcome to try out your strategy
2. Use QA pre-trained models to evaluate the quality of your dataset
* Investigate different strategies and metrics in the literature to evaluate Q&A dataset
* Don't use the same model for both data generation and evaluation. For example, if you fine-tune model A, then you must use model B (and so on) to evaluate the quality of the dataset
3. Document your code and final report

#### **Extra Tasks:**

Below are some questions that snalADDY is interested in, but it is not an exhaustive list. You can come up with additional tasks that you think they are hard and important:

* Text summarization for more efficient interaction:
  * Combine related questions (e.g., company size, industry, product focus) into a single query
  * Ensure accurate mapping of answers to original questionnaire fields
* Information Retrieval for Multi-Select Questions:
  * Transform unstructured time expressions (e.g., “next week”) into precise dates using LLMs
* Detection and Handling of Missing Responses:
  * Create a method to identify intentional skips versus missing relevant information

#### **Minimal Passing Criteria:**

* Generate your sample data
* Apply at least a QA-model
* Evaluate the performance (investigate suitable metrics for Q&A task)
* Provide a documentation of the code and project:
  * Powerpoint presentation AND
  * Word/PDF Document **AND/OR** Jupyter Notebooks **AND/OR** Online Package Documentation (readthedocs.com)
  * Documentation must include the responsibilities of the individual team members

#### **General Criteria:**

* Variety of implemented models & benchmarks
* Quality of the evaluation
* Variety of tested scenarios (e.g., responses of different quality/difficulty)
* Description of further steps (how could models be improved, what else could be done)
* Originality of the analyses
* Functionality frontend/dashboard
* Number of extra questions considered

#### **Final Submissions:**

* (MUST) submit a runnable notebook that contains all of the code of your project, similar to the style of the lectures
* (MUST) submit a pdf/word document describing the contents of your project. Please indicate individual contributions, as your performance will be graded individually 
* (Optional) use readthedocs instead of pdf/word document

All submissions should be zipped and uploaded onto wuecampus under the "Submission" tab. Only one student in the group needs to submit the project.
