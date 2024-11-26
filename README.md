# GenAI
Medical Research Assistant

## Recap
- Description: 
Develop a system to answer questions about specific medical conditions or treatments based on a corpus of research papers, clinical guidelines, and pharmaceutical data.
- Use Case:
Assist medical professionals or patients in finding evidence-based information about rare diseases, treatment plans, or drug interactions.
- Challenges:
Medical terminologies, ensuring safety-critical answers, handling legal and ethical concerns in providing health-related advice.



## Main criteria

The main criteria for the Medical Research Assistant LLM would include:
1. Answer Quality Metrics
- Accuracy:
	- Definition: Measures whether the system provides correct and evidence-based information.
	- Relevance: In a medical context, accuracy is absolutely essential because the wrong information can have serious or even life-threatening consequences. It's critical for legal and ethical reasons to ensure the system is trustworthy. The system must be able to accurately extract and present data from clinical guidelines, research papers, and pharmaceutical databases.
	- Evaluation: This can be measured by comparing system-generated answers against verified clinical guidelines or subject-matter expert reviews. Additionally, medical professionals can rate the quality of responses to ensure accuracy.
- Completeness:
	- Definition: Evaluates whether the system provides answers that are thorough and fully address the user’s query.
	- Relevance: In the context of rare diseases or complex treatment plans, incomplete answers could lead to misinformed decision-making. The system must offer comprehensive information, especially when handling safety-critical answers.
	- Evaluation: This can be tested by tracking how often users ask follow-up questions for clarification, which may indicate the initial answer was incomplete.

2. User Experience Metrics
- Response Time:
	- Definition: The time it takes for the system to return an answer after a query is submitted.
	- Relevance: Medical professionals often require quick access to information, especially in clinical settings where time is critical. A system that is too slow could impede decision-making, making it less useful.
	- Evaluation: Benchmark response times and aim to keep them within an acceptable range (e.g., less than 2 seconds for basic queries).
- Ease of Use (Usability):
	- Definition: How intuitive and user-friendly the system interface is for end-users.
	- Relevance: Both medical professionals and patients might use this system, so it needs to be accessible to users with varying levels of medical knowledge. If the system is difficult to navigate or requires excessive effort to retrieve information, user adoption will be lower.
	- Evaluation: This can be evaluated through usability tests, user feedback, and surveys. You can also track user behavior (e.g., task completion rates) to see if users are struggling.

3. Performance Metrics
- Scalability:
	- Definition: Measures how well the system handles an increasing number of users or a growing corpus of research papers without degrading performance.
	- Relevance: As the system grows in popularity or incorporates more data, it must continue to provide accurate and timely responses. If it cannot scale, performance issues (like slow response times or system crashes) could occur, reducing reliability.
	- Evaluation: Load testing under simulated peak usage conditions can determine how well the system scales. For instance, you can monitor latency and throughput as the system processes more queries.
- Data Freshness (Timeliness of Updates):
	- Definition: How frequently and quickly the system updates its corpus to include new medical research, guidelines, or pharmaceutical information.
	- Relevance: Medical knowledge is constantly evolving, with new research and treatment protocols emerging regularly. The system must be able to incorporate these updates quickly to remain relevant and accurate.
	- Evaluation: Track how long it takes to incorporate new data and measure whether queries reflect the most current guidelines and research.

4. Cost Metrics
- Operational Costs:
	- Definition: The costs associated with running and maintaining the system, including computing resources, storage, and data acquisition.
	- Relevance: It's important to keep operational costs manageable, especially if the system is widely used or free for users. Cloud hosting, data storage, and AI processing (like natural language models) can become expensive at scale.
	- Evaluation: Monitor monthly or yearly costs for data storage, compute, and any associated licensing fees for accessing proprietary medical databases. Optimize resources to reduce unnecessary expenditures (e.g., scaling servers dynamically based on usage).
- Development and Maintenance Costs:
	- Definition: The costs of developing new features, bug fixes, and general maintenance of the system.
	- Relevance: The system may require regular updates to ensure it meets the needs of users and complies with evolving regulations. High development costs might make the system unsustainable in the long run.
	- Evaluation: Track development hours, maintenance schedules, and resource allocation for bug fixes. Analyze whether there's a high cost for changes or new feature implementations.

Each of these metrics addresses a specific challenge or goal in developing a medical research assistant system:
- Answer Quality Metrics ensure that the system provides accurate, reliable, and thorough responses—essential for safety-critical environments.
- User Experience Metrics focus on how effectively users can interact with the system and receive information in a timely manner, which is vital in medical decision-making.
- Performance Metrics help assess the system’s ability to scale and stay up-to-date with the latest medical research, ensuring long-term viability and reliability.
- Cost Metrics aim to keep the system financially sustainable, ensuring that it remains accessible to users without incurring prohibitive operational costs.
These metrics, when measured and optimized, help ensure that the system provides high-quality, timely, and cost-effective assistance for medical professionals and patients alike.

## Q&A

[link to Q&A file](https://www.kaggle.com/datasets/gvaldenebro/cancer-q-and-a-dataset?resource=download&select=growth_hormone_receptorQA.csv)

[link to the selected Q&A](https://docs.google.com/spreadsheets/d/10wujNUzXb3qMbppAO7kucGEroBbA6WZmSpmzudxlZuI/edit?usp=sharing)

## Benchmarks for Your Medical Research Assistant Project
From the reviewed benchmarks, here are the top 5 that are most pertinent to your project's use case:

|**Benchmarks**|**Description**|**Link**|**Relevance**|
|--------------|---------------|--------|-------------|
|BLURB (Biomedical Language Understanding & Reasoning Benchmark)|BLURB is a collection of tasks that evaluate the ability of language models to understand and reason over biomedical texts. It consists of tasks like named entity recognition (NER), relation extraction (RE), sentence similarity, and question-answering tailored specifically for biomedical literature.| [Link](https://microsoft.github.io/BLURB/) |BLURB is highly relevant to the GenAI Medical Research Assistant because it focuses on evaluating models for biomedical natural language processing (NLP), which is crucial when dealing with medical terminologies, drug names, and clinical guidelines. It helps in assessing how well the assistant can process, understand, and answer questions from medical research and clinical guidelines.|
|MedQA|MedQA is a benchmark designed to evaluate AI models on medical question-answering tasks using content from the United States Medical Licensing Examination (USMLE). It consists of questions that require deep medical knowledge, spanning multiple-choice questions typically used in medical exams.|[Link](https://github.com/jind11/MedQA)|MedQA is important because it simulates the real-world scenario where medical professionals ask diagnostic or treatment-related questions. The assistant's ability to answer these questions accurately ensures it can provide reliable, evidence-based information to both medical professionals and patients.|
|PubMedQA|PubMedQA is a question-answering dataset derived from PubMed articles. It includes questions focused on biomedical research, where answers are fact-based and sourced from abstracts of PubMed papers. It consists of questions in three categories: yes/no questions, factoid questions, and open-ended questions.|[Link](https://pubmedqa.github.io)|PubMedQA is relevant because it is based on real medical research publications. The GenAI system can use it to benchmark its ability to provide accurate and evidence-based answers from biomedical literature. This is critical for ensuring that the assistant delivers precise information backed by research.|
|ChEMBL|ChEMBL is a large-scale bioactivity database containing information on drug-like small molecules, including their chemical properties, bioactivity, and associated targets. It is widely used for drug discovery and pharmacological research.|[Link](https://www.ebi.ac.uk/chembl/)|For a Medical Research Assistant providing drug information, ChEMBL serves as an important benchmark to evaluate the system’s ability to retrieve and process chemical and pharmacological data. It's crucial for answering drug interaction questions, supporting evidence-based treatment plans, and identifying drug efficacy or toxicity.|
|SQuAD (Stanford Question Answering Dataset)|SQuAD is a well-known reading comprehension dataset where a system must extract the answer to a question from a given passage of text. The dataset includes questions with corresponding passages from Wikipedia.|[Link](https://rajpurkar.github.io/SQuAD-explorer/)|While SQuAD is not medical-specific, it provides a general-purpose benchmark for question-answering. The ability of the Medical Research Assistant to perform well on SQuAD can indicate its potential for robust language understanding, comprehension, and answer extraction, which are transferable skills to the medical domain when answering research-related questions.|


## Benchmarks 

I was unable to find specific benchmark scores for Orca Mini 3B on the datasets you mentioned (BLURB, MedQA, PubMedQA, CHEMBL, and SQuAD). However, I can provide insights from similar models in terms of size and scope.


|Benchmark|	Orca Mini 3B (Assumed)|	Similar Models (LLaMA-3-8B)	|Other Relevant Models (7B-8B)|
|--------------|---------------|--------|-------------|
|BLURB	|N/A	|Not directly found	|70-75 (7B Medical models)|
|MedQA	|N/A	|73.3 (LLaMA-3-8B, Greedy)	|60-77 (Med-PaLM, OpenBioLM)|
|PubMedQA|	N/A	|77.0 (LLaMA-3-8B, Greedy)|	74.1 (OpenBioLM-8B)|
|CHEMBL	|N/A	|Not available	|Not found for models of this size|
|SQuAD	|N/A	|Not found	|80-85 (similar 7B-8B models)|

![image](https://github.com/user-attachments/assets/cab4f309-d9a8-4ef9-ac94-c89304ea5459)

[lien test](https://huggingface.co/pankajmathur/orca_mini_3b)
[Open Medical-LLM](https://github.com/huggingface/blog/blob/main/leaderboard-medicalllm.md)
[Llama-3-8B-UltraMedical](https://huggingface.co/TsinghuaC3I/Llama-3-8B-UltraMedical)

## Fine-Tuning

Here is a table summarizing the details of the **ClinicalBERT** model from Hugging Face:

| **Attribute**               | **Details**                                                                                       |
|-----------------------------|---------------------------------------------------------------------------------------------------|
| **Link**                    | [ClinicalBERT on Hugging Face](https://huggingface.co/medicalai/ClinicalBERT)                     |
| **Documentation Quality**    | Basic overview provided with usage instructions, pretraining data, and citation information.       |
| **Fine-tuned to**            | Clinical data, specifically Electronic Health Records (EHRs) from over 3 million patient records. |
| **Base Model**               | BERT (Bidirectional Encoder Representations from Transformers).                                   |
| **Benchmark Scores**         | Not available on the model card.                                                                  |
| **Available in GGUF (Ollama)**| Not listed as available in GGUF format.                                                           |

