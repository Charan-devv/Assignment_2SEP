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

### **Requirement 3: Balanced Training Data**  
- **User Requirement:**  
  *As an AI developer, I want the system to detect bias in training data so I can ensure fair AI models.*

  #### **Assumptions & Validation:**  
- **Assumption:** Finding and fixing bias in data will make AI models more accurate and reliable.  

##### **Validation Methods:**  
1. Analyze past training data for bias patterns.  
2. Compare AI model accuracy before and after fixing bias.  
3. Get developer feedback on bias detection reports.

#### **Preliminary Tasks:**  
1. Identify common bias issues in AI training datasets.  
2. Research available AI fairness and bias detection tools.  
3. Develop a prototype bias detection system for testing.

#### **Functional Requirements:**  
1. The system shall scan training datasets for bias indicators, such as overrepresentation or underrepresentation of certain groups.  
2. The system shall generate a bias detection report highlighting potential fairness issues.  
3. The system shall allow users to adjust dataset parameters to correct detected biases before model training.  
4. The system shall provide visualizations to help developers understand bias trends in the dataset.

#### **System Requirements:**  
1. The system shall use AI-based fairness detection tools to analyze dataset distribution.  
2. The system shall integrate predefined fairness metrics such as demographic parity and equal representation.  
3. The system shall provide a dashboard with real-time bias monitoring and suggested actions to correct imbalances.  
4. The system shall support integration with third-party bias detection frameworks for extended functionality.

### **Requirement 4: Reports on Data Balance**
- **User Requirement:**  
  *As an AI developer, I want reports on data balance so I can check if my training data is fair and make improvements if needed.*

  #### **Assumptions & Validation:**  
- **Assumption:** Developers will benefit from clear reports that highlight fairness issues in datasets.  

##### **Validation Methods:**  
1. Test if reports help developers make better data decisions.  
2. Compare AI performance before and after using balanced datasets.  
3. Collect feedback on the clarity and usefulness of reports.

#### **Preliminary Tasks:**  
1. Research best practices for visualizing dataset balance.  
2. Define what data balance indicators should be included in reports.  
3. Test different reporting formats with developers.  
4. Develop an initial reporting prototype and refine based on feedback.

#### **Functional Requirements:**  
1. The system shall generate detailed reports on dataset balance, highlighting overrepresented and underrepresented groups.  
2. The system shall provide recommendations on how to rebalance biased training data.  
3. The system shall allow users to schedule automated dataset balance reports.  

#### **System Requirements:**  
1. The system shall use data analytics tools to process and visualize dataset balance information.  
2. The system shall integrate with reporting tools to generate customizable insights.  
3. The system shall provide an API for external applications to fetch bias analysis reports.