# NER model in health tech

# Problem Statement

## Description
BeHealthy, a health tech company, aims to connect medical communities with patients through a web platform. The platform enables doctors to list services, manage patient interactions, and provide services like booking appointments and ordering medicines online. However, understanding medical terms in patient notes can be challenging for non-medical professionals. The goal of this project is to build a custom Named Entity Recognition (NER) model to identify disease names and their possible treatments from medical data.

### Challenges

1. **Medical Terminology**: Medical notes contain specialized terminology that can be difficult for non-medical professionals to understand. The NER model needs to accurately identify and extract these terms.
2. **Data Volume**: BeHealthy generates large volumes of data from medical services, prescriptions, and online consultations. The NER model should be able to handle this large volume of data efficiently.
3. **Data Quality**: Medical data can be noisy and contain errors. The NER model needs to be robust enough to handle these issues and provide accurate results.
4. **Generalization**: The model should be able to generalize well to new and unseen medical terms and treatments.

### Objectives

1. **Build a Custom NER Model**: Develop a NER model specifically tailored to identify disease names and treatments from medical data.
2. **Improve Patient Care**: By accurately identifying diseases and treatments, the platform can help improve patient care and treatment outcomes.
3. **Enhance User Experience**: Providing doctors with an easy-to-use platform for managing patient interactions and medical records can enhance the overall user experience.
4. **Support Decision Making**: The platform can support doctors in making informed decisions about patient care by providing them with relevant information about diseases and treatments.
5. **Enable Data-Driven Insights**: Analyzing the extracted data can provide valuable insights into disease prevalence, treatment effectiveness, and other healthcare trends.

### Expected Outcome

- A robust NER model that accurately identifies disease names and treatments from medical data.
- Improved efficiency and accuracy in managing patient interactions and medical records.
- Enhanced user experience for doctors using the BeHealthy platform.
- Data-driven insights that can support decision-making in patient care and treatment planning.

# Task List

1. **Data Preprocessing**:
   - Construct sentences from tokenized data.
   - Organize words into coherent sentences and display a sample of sentences with their corresponding labels.

2. **Concept Identification**:
   - Use PoS tagging to identify common concepts.
   - Output the top 25 most frequently discussed concepts.

3. **Defining CRF Features**:
   - Define features with PoS tags.
   - Consider the preceding word for context.
   - Mark the first and last words in a sentence.

4. **Feature Extraction**:
   - Write code to extract feature values for each sentence.
   - Get a list of labels for each preprocessed label line.

5. **Input and Target Variables**:
   - Extract features as input for the CRF model.
   - Extract labels as the target variable.

6. **Building the CRF Model**:
   - Build the CRF model using sklearn.

7. **Evaluation**:
   - Predict labels for tokens in the test data.
   - Calculate the F1 score using actual and predicted labels.

8. **Identifying Diseases and Treatments**:
   - Create code to get all predicted treatments corresponding to each disease label in the test data.
   - Predict the treatment for the disease "hereditary retinoblastoma."

