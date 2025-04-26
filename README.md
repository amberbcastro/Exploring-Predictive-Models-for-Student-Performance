![Grade Logo](https://github.com/user-attachments/assets/3f6d9f0e-31bf-426a-8834-5e05d9c12180)

# Exploring Predictive Models for Student Performance: A Case Study in Life Science Calculus I Exam Data Modeling

## 1Real-World Problem Statement
**Full statement of the problem:**  
Can we build predictive models using Exam 1 and Exam 2 scores to estimate student performance in Calculus I? 

Since final grades are not yet available, we will compare the outputs of multiple modeling approaches to understand their assumptions, behaviors and potential for future use.

## Assumptions
1. **Exam scores reflect student learning and effort.**  
   Exams are standardized and graded consistently.  
2. **In absence of final grade data, Exam 3 can serve as a proxy** for overall performance.  
3. **All exam scores use a consistent scale.**
4. **All exams cover the same amount of content**
5. **All exams have the same difficulty**
6. **Content delivered to students consistently throughout the semester**

*Why these are sensible:*  
- Midterm exams are major components of grade and correlate with understanding.  
- Using Exam 3 avoids waiting for end-of-term grades.  
- Consistent scales ensure comparability across models.

## Modeling Setup and Dataset Information
The dataset was obtained from the USF Life Science Calc student I section 002. Students are all taught by the same professor and exams are graded by the same graders.
### Variables
For the purposes of this project, the following variables were analyzed:
| Variable Name   | Description                              | Type     | Default Value |
|-----------------|------------------------------------------|----------|---------------|
| `SID`| Student ID | `number` | `123456788` |
| `Total Score`| Student's score on Exam | `number` | `98` |
| `Max Points`| Highest amount of Points a student could obtain | `number` | `105` |
| `Status`| Whether exam was graded or missing | `string` | `Graded or Missing` |


## Mathematical Tools

## The Simplest Version

## Variations of the Problem

## The Pitch
