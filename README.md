# Examination System Design

This document outlines the business case and requirements for an Examination system for our organization.

## System Requirements

### 1. Question Class Design
The Question object should consist of:
- Header of the question
- Body of the question
- Mark

### 2. Exam Types
The system supports two types of exams:
- Final Exam
- Practical Exam

### 3. Question Types
Different question types for each exam:
#### Final Exam:
- True or False
- MCQ (Multiple Choice Question - single answer)

#### Practical Exam:
- MCQ (Multiple Choice Question)

*Note*: Implement a Base Question class with specific question types as inherited classes.

### 4. Answer Class
Define a class for answers containing:
- AnswerId
- AnswerText

### 5. Question-Answer Relationship
- Each Question is associated with:
  - An array of answers (Answers[] AnswerList)
  - Designation of the correct answer

### 6. Base Exam Class
Design a Base Exam class with common attributes:
- Time of exam
- Number of Questions
- Show Exam Functionality (different implementation for each exam type)

### 7. Subject Class
Every Exam object is associated with a Subject class containing:
- Subject Id
- Subject Name
- Exam of the subject
- Functionality to create the subject's exam

### 8. Practical Exam Features
- Shows the right answer after exam completion

### 9. Final Exam Features
- Shows:
  - Questions
  - Answers
  - Grade

### 10. Main Implementation
- Declare a subject object in Main
- Create one type of exam using the subject object
