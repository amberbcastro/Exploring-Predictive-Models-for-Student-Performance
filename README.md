![Grade Logo](https://github.com/user-attachments/assets/3f6d9f0e-31bf-426a-8834-5e05d9c12180)

# Exploring Predictive Models for Student Performance: A Case Study in Life Science Calculus I Exam Data Modeling

## Real-World Problem Statement
**Full statement of the problem:**  
With final exams quickly approaching, students are often dreading the finals grind filled with lots of caffeine and an overwhelming amount of studying. Professors are equally yearning for the semester’s close as class attendance dwindles and assignments to finish grading stack up. 

But are final exams an accurate representation of student knowledge and performance in a course – or can we just accept the exams taken during the semester as good enough?

## Assumptions
1. **Exam scores reflect student learning and effort.**  
   Exams are standardized and graded consistently.  
2. **In absence of final grade data, Exam 3 can serve as a proxy for overall course performance.**  
3. **All exam scores use a consistent scale.**
4. **All exams cover the same amount of content**
5. **All exams have the same difficulty**
6. **Content delivered to students consistently throughout the semester**

*Why these are sensible:*  
- Midterm exams are major components of final grade calculation and correlate with understanding.  
- Using Exam 3 avoids waiting for end-of-term grades to meet our project deadline.  
- Consistent scales ensure comparability across models.

## Modeling Setup and Dataset Information
The dataset was obtained from the USF Life Science Calculus I section 002 of Spring 2025. It contains information on students' exam scores for exams 1, 2 and 3. Students are all taught by the same professor and exams are graded by the same 4 graders. **Please note that the dataset is not included here because it contains sensitive information, and this page is publicly accessible.**
### Variables 
For the purposes of this project, the following variables were analyzed:
| Variable Name   | Description                              | Type     | Example Value |
|-----------------|------------------------------------------|----------|---------------|
| `SID`| Student ID | `number` | `123456788` |
| `Total Score`| Student's score on Exam | `number` | `98` |
| `Max Points`| Highest amount of Points a student could obtain | `number` | `105` |
| `Status`| Whether exam was graded or missing | `string` | `Graded or Missing` |

### Summary statistics of Dataset
Number of students: 160 
| Variable Name   | Exam 1     | Exam 2     | Exam 3     |
|-----------------|----------|----------|----------|
| `Mean`|  `59.163` | `73.064` | `fill in later` |
| `Q1`|  `42.5` | `59.875` | `fill in later` |
| `Q3`|  `78.0` | `90.125` | `fill in later` |
| `Median`| `57.5` | `76.0` | `fill in later` |
| `Maximum`|  `104.0` | `107.0` | `fill in later` |
| `Minimum`|  `5.5` | `10.0` | `fill in later` |
| `Count of Missing`|  `7` | `12` | `fill in later` |
| `Max Points (Available)`|  `105` | `107` | `fill in later` |





## Mathematical Tools

## The Simplest Version

## Variations of the Problem

## The Pitch
