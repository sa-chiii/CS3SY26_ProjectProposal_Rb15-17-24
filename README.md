# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template: 

### Project Title or Name of the Application	: The Tomsup Pet Shop
### Section			   	      : 9-Rubidium
### Group Members			    : LOARES, Cleo, MAGHUYOP, Lia, REMIGIO, Luis
### Date (Proposal Date)  : Nov 12, 2026

### Project Description:

- The PISAYMaxxer helps PISAY students of any grade keep track of requirements and their current GWA with the use of OOP.

**How does it work?**
- In this program, we have 4 classes: 
    1. _class Student_ - this serves as the top level user profile. Its has private attributes (data) which are: student_name (str), batch (str), and subjects (list). It's public methods includes add_subject(), remove_subject(), and calculate_GWA().
    2. _class Subject_ - blue print for all courses, it stores all units, list of requirements, and converts percentages to the 1.00–5.00 scale. Its private attributes include: subject_name (str), units (float), weights (dictionary), and tasks (list). Its methods include: add_task(), get_pending_task(), compute_quarter_grade(), compute_cumulative_grade(), and convert_pisay_grade().
    3. _class Requirement_ - represents ungraded tasks, reminders, or deadlines. Its private attributes include: title (str), due_date (str), quarter (int: 1-4), and is_done (bool). Its methods include: mark_done(), get_title(), get_due_date(), get_quarter(), and get_info().
    4. _class GradedTask_ - child class and inherits from Requirement; adds scores and assessment categories (e.g., Quiz, Lab, Long Test, Periodic Exam). Its private attributes includes: the inherited attributes, category (str), score (float), and max_score (float). Its methods include: record_score(), get_category(), get_score(), get_max_score(), and get_info() (overridden)

- The Student class contains a list of Subject instances. To find the GWA of the quarterly/cumulative, the program goes through the subjects, multiplies its 1.00–5.00 grade with its units, and then divides it by the total units.
- In the case of compute_quarter_grade(), the Subject class gets all completed tasks for the quarter, gets the weighted percentage, and then converts it to a 1.00–5.00 grade using an internal private helper method convert_pisay_grade() to avoid messy main program.
- A plain reminder is stored in the Requirement object while the graded tasks such as quiz and exam are stored in the GradedTask object. GradedTask inherits the title, due date, quarter, and mark_done() methods from Requirement via super().__init__().
- Requirement and GradedTask both have the get_info() method, although they display different information. Requirement.get_info() displays a plain reminder while GradedTask.get_info() overrides it to display the category and score.

**Who are our target users?**
- The primary demographic of this application are Junior to Senior High School students enrolled in Grade 7 to Grade 12 (ages 12-18 years old). JHS students benefit from tracking 8-10 subjects quarterly, and SHS students will be aided by having reduced burdens from their heavy semester based work loads with regard to weighted scores per strand, plus the demands of research paper writing and capstone projects. The tool helps both JHS and SHS in that way.

- The description is then followed by the class diagram, depicting clearly what was described.

**Sample class Diagram from https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png:**

![Sample Diagram](https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png)

### Goals:
With the help of PISAYMaxxer, we aim to help student users and developers alike. For students, the program will help them improve time management and self-regulation. Using a single tool to view both upcoming tasks and academic standing (catered for pisay students) will encourage students to take proactive initiative, build the habit of knowing what they need to prioritize, and reduce academic stress. Additionally, because the program is built with OOP concepts, it is easy to add features, create developments, and improve the experience as years go by. 

- Objective 1: To develop an object-oriented system with the basic principles of OOP for handling students' profiles, subject offerings, and organized academic requirements.

- Objective 2: To create a module for task tracking with deadline reminders so that students can prioritize their academic tasks per subject and avoid missing deadlines as well as cramming on academic requirements.

- Objective 3: To add an automated GWA Calculation and Grade Simulation feature that will be able to calculate the weighted average grade according to the subject's units and be able to project the student’s academic standing with the next set of academic requirements.

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
