# DBMS-Expt01

## Aim
To analyze the problem and come with the entities in it and identify the constraints in creating the database.

### Scenario 1: University Database
Consider a university database system designed to manage information about students, courses, instructors, and the enrollment of students in courses. The university offers various programs, and each program consists of multiple courses.

User Requirements:

The university offers various academic programs that are grouped under different departments. Details that need to be captured for each program include a unique identifier, program name and the governing department.

The university has a list of students enrolled across different programs offered. For every student, details like unique admission number, full name, date of birth, contact information such as email and phone number need to be stored.

There are multiple instructors in the university teaching one or more courses. Relevant details for each instructor required include unique staff number, name, contact information like phone and email.

The university offers a catalog of courses across programs. Each course taught requires capturing course number, name, number of credits/units etc.

Students can enroll or register in one or more courses in a given academic term. The system needs to track details like which student has enrolled in which particular course(s) and date of enrollment for reporting requirements.

Tasks:

Create an ER diagram for the University Database based on the given scenario.

Identify entities, relationships, and attributes.
Specify cardinality and participation constraints.
Extend the ER diagram to include the concept of prerequisites for courses.

Consider the fact that certain courses may have prerequisites.
Explain your design choices and assumptions.

Provide a brief explanation of why you chose certain entities, relationships, and how you addressed the concept of prerequisites.
#### ER Diagram
![Entity Relationship Diagram Team Whiteboard](https://github.com/Harsayazheni/DBMS-Expt01/assets/118708467/8a7a76c0-e4a0-42ab-9a6e-06cf36041421)

#### Explanation
Entities:

Student: Represents an individual enrolled in a university program.
Course: Represents a specific academic course offered by the university.
Program: Represents a degree program or major offered by the university.
University: Represents the institution itself.
Department: Represents a specific department within the university.
Mentor: Represents a faculty member or advisor assigned to a student.
Relationships:

A Student is enrolled in a Program.
A Program is offered by a University.
A Course is part of a Program.
A Course has Prerequisites, which are other courses that must be completed before taking the course.
A Student has Attempts at a Course, which represents their enrollment and grade history.
A Department offers Courses.
Prerequisites:

The concept of prerequisites is implemented through the Contains relationship between Courses. This allows for the representation of hierarchical dependencies between courses, where a course may have one or more prerequisites that must be completed before it can be taken. For example, a course in calculus may have a prerequisite of algebra, indicating that students must complete algebra before enrolling in calculus.

The Prerequisites relationship is likely implemented as a many-to-many relationship, allowing a course to have multiple prerequisites and a prerequisite course to be required for multiple courses.

Overall, this entity-relationship model appears to be designed to manage student enrollment, course offerings, and program requirements, while also ensuring that students meet the necessary prerequisites for each course.

## Result 
Thus ,To analyze the problem and come with the entities in it and identify the constraints in creating the database is done successfully.
