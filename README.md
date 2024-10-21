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

- Accuracy and Reliability: The assistant must provide highly accurate, evidence-based answers derived from research papers, clinical guidelines, and pharmaceutical data. This is crucial in delivering safe and trustworthy medical advice, especially in cases involving rare diseases and treatment plans.
- Medical Terminology Comprehension: The system should have a deep understanding of complex medical terminologies to effectively interpret and convey specialized medical knowledge to both healthcare professionals and patients.
- Safety-Critical Answers: It should prioritize patient safety by clearly identifying approved treatments, highlighting drug interactions, and offering guidance within the bounds of clinical best practices. This includes recognizing when to escalate a query for professional consultation rather than offering potentially harmful advice.
- Legal and Ethical Compliance: The assistant must adhere to relevant legal and ethical standards in health communication, such as ensuring patient privacy (HIPAA, GDPR compliance) and avoiding misdiagnosis or unqualified advice.
- User-Specific Customization: The model must be able to adjust its language and detail level based on the user's background, whether they are a medical professional seeking in-depth details or a patient requiring simplified, layperson-friendly explanations.
- Data Handling and Up-to-date Information: The system must efficiently handle a large corpus of medical research, keeping answers current with the latest findings and treatment guidelines, especially in rapidly evolving medical fields.

## Q&A

[link to Q&A](https://www.kaggle.com/datasets/gvaldenebro/cancer-q-and-a-dataset?resource=download&select=growth_hormone_receptorQA.csv)

https://docs.google.com/spreadsheets/d/10wujNUzXb3qMbppAO7kucGEroBbA6WZmSpmzudxlZuI/edit?usp=sharing

## Benchmarks

Top 5 Benchmarks for Your Medical Research Assistant Project
From the reviewed benchmarks, here are the top 5 that are most pertinent to your project's use case:

- BLURB - for its focus on various biomedical tasks, making it ideal for handling medical terminologies and evidence-based content.
- MedQA - because it directly tests the model's ability to answer clinical and patient-centric questions.
- PubMedQA - for evaluating how well the model can assist in reviewing and summarizing research papers.
- CHEMBL Benchmark - necessary for evaluating drug interactions, an essential component in pharmaceutical data handling.
- SQuAD - for a broader evaluation of comprehension and question-answering abilities, adaptable to general medical queries.
![image](https://github.com/user-attachments/assets/cab4f309-d9a8-4ef9-ac94-c89304ea5459)


[lien test](https://huggingface.co/pankajmathur/orca_mini_3b)
