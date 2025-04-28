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
3. **All exams cover the same amount of content**
4. **All exams have the same difficulty**
5. **Content delivered to students consistently throughout the semester**

*Why these are sensible:*  
- Midterm exams are designed to test core course material, so their scores should reflect student learning and effort.  
- Using Exam 3 as a stand-in for final performance allows us to move forward without needing official final grades, which fits within our project timeline.  
- Assuming all exams cover the same amount of material and are equally difficult makes it reasonable to compare scores directly across exams.  
- Consistent delivery of content throughout the semester supports the idea that exam scores measure the same skills and knowledge at each point.  
- Standardized grading ensures that differences in scores are due to student performance rather than grading inconsistencies.

## Modeling Setup and Dataset Information
The dataset was obtained from the USF Life Science Calculus I section 002 of Spring 2025. It contains information on students' exam scores for exams 1, 2 and 3. Students are all taught by the same professor and exams are graded by the same 4 graders. 

**Please note that the dataset is not included here because it contains sensitive information, and this page is publicly accessible.**

### Variables 
For the purposes of this project, the following variables were analyzed:
| Variable Name   | Description                              | Type     | Example Value |
|-----------------|------------------------------------------|----------|---------------|
| `SID`| Student ID | `number` | `123456788` |
| `Total Score`| Student's score on Exam | `number` | `98` |
| `Max Points`| Highest amount of Points a student could obtain | `number` | `105` |
| `Status`| Whether exam was graded or missing | `string` | `Graded or Missing` |

### Summary Statistics of the Dataset
Number of students: 160 
| Variable Name   | Exam 1     | Exam 2     | Exam 3     |
|-----------------|----------|----------|----------|
| `Mean`|  `59.163` | `73.064` | `66.531` |
| `Q1`|  `42.5` | `59.875` | `58.25` |
| `Q3`|  `78.0` | `90.125` | `77.75` |
| `Median`| `57.5` | `76.0` | `67.0` |
| `Maximum`|  `104.0` | `107.0` | `102.0` |
| `Minimum`|  `5.5` | `10.0` | `15.0` |
| `Count of Missing`|  `7` | `12` | `33` |
| `Max Points (Available)`|  `105` | `107` | `105` |

![Box_Plot_Exams](graphs/box_plot_exam_scores.png)

**Please Note:**
- Because each exam had a different maximum number of points available (e.g., 105, 107), **all exam scores were converted to percentages to ensure comparability across exams.**
- **Students missing a grade for any of the three exams were excluded from the final dataset.** This decision was made to maintain consistency in the analysis and to ensure that all models were trained and evaluated on complete information.

## Mathematical Tools

- **Linear Regression**  
  - **Why:** To predict a student’s Exam 3 score using their Exam 1 and Exam 2 scores.  
  - **How:** We draw the best straight line through the data points so it’s as close as possible to all the exam scores.

- **Logistic Regression**  
  - **Why:** 
  - **How:** 

- **K-Means Clustering**  
  - **Why:** To find natural groups of students based on their three exam scores.  
  - **How:** We pick a number of groups (k), place a point for each group, assign students to the closest point, then move those points to the average of their assigned students until it stops changing.

- **Cross-Validation**  
  - **Why:** To check if our models work well on new data.  
  - **How:** We split the data into parts, train the model on some parts and test on the rest, then repeat for each part and average the results.

- **Silhouette Analysis**  
  - **Why:** To see how clear the clusters are.  
  - **How:** We measure for each student how close they are to their own group compared to the next closest group, then average those scores.


## The Simplest Version

## Variations of the Problem

## The Pitch
