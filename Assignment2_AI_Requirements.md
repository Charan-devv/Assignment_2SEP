# **Assignment 2: Requirements**

## **Purpose**  
This Assignment defines user, functional, and system requirements for an AI developer who collects training data using web scraping. The goal is to categorize training questions properly and ensure training data is fair to improve AI model performance.

---
## **Scenario Summary**  
The AI developer faces two main challenges:  
1. **Training questions need to be categorized and stored separately from answers** to help developers focus and improve learning.  
2. **Training data should be fair and unbiased** to create better AI models.  

Our goal is to define clear requirements to solve these problems.  

---

## **User, Functional & System Requirements**  

### **Requirement 1: Categorized Training Questions**  

- **User Requirement:**  
  *As an AI developer, I want training questions to be grouped by category so I can quickly find relevant data for AI training.*

  #### **Assumptions & Validation:**  
- **Assumption:** Categorized questions will help developers find relevant data faster.  

##### **Validation Methods:**  
1. Ask developers if categorized data improves workflow.  
2. Compare search times for categorized vs. uncategorized questions.  
3. Test categorized questions with developers and gather feedback.

#### **Preliminary Tasks:**  
1. Identify common categories used in training datasets.  
2. Review existing AI-based categorization tools.  
3. Define rules for how questions should be categorized. 

#### **Functional Requirements:**  
1. The system shall allow users to assign categories to training questions manually.  
2. The system shall automatically classify training questions into predefined categories using AI-based text analysis.  
3. The system shall enable users to search and filter training questions based on category.

#### **System Requirements:**  
1. The system shall use a relational database to store categorized training questions separately from other data.  
2. The system shall implement an AI-powered text classifier to categorize questions based on content and context.  
3. The system shall provide a search and filtering mechanism to retrieve training questions by category.

### **Requirement 2: Separating Questions and Answers** 
- **User Requirement:**  
  *As an AI developer, I want training questions stored separately from answers so I can focus on problem-solving without seeing answers immediately.*

  #### **Assumptions & Validation:**  
- **Assumption:** Keeping questions and answers separate will help developers think critically and reduce bias.

##### **Validation Methods:**  
1. Compare AI model performance trained with mixed vs. separated question-answer data.  
2. Conduct developer interviews to determine the impact of answer separation.  
3. Test if separation improves developer learning and AI model accuracy. 

#### **Preliminary Tasks:**  
1. Study how developers currently interact with training questions and answers.  
2. Research best database structures for separate storage.  
3. Define rules for when users can access answers.  

#### **Functional Requirements:**  
1. The system shall store training questions in a separate database table from answers.  
2. The system shall allow users to access training questions without answers by default.  
3. The system shall include a toggle option that lets users view or hide answers when reviewing training questions.

#### **System Requirements:**  
1. The system shall use a structured relational database to store questions and answers in separate tables.  
2. The system shall implement an access control mechanism to prevent unauthorized users from viewing answers.  
3. The system shall log when and by whom an answer is viewed or modified.