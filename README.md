# CS 255: System Analysis and Design Portfolio

## 📘 Course Overview
This repository contains coursework and projects completed for CS 255: System Analysis and Design at Southern New Hampshire University. The course focuses on the principles, methods, and techniques used in systems development, including the creation of system models and effective communication of technical concepts.

## 🧠 Course Competencies
- **CS-30404**: Explain the principles, methods, and techniques of systems development.
- **CS-30405**: Create various system models through the application of appropriate tools.
- **COM-20257**: Present and articulate technical concepts to nontechnical audiences.

## 📂 Repository Contents
- `ProjectOne/`: Requirements gathering, process modeling, and object modeling artifacts.
- `ProjectTwo/`: UML diagrams and presentation materials for nontechnical audiences.
- `Assignments/`: Weekly assignments covering SDLC, modeling techniques, and system evaluation.
- `Discussions/`: Reflections and insights from weekly discussion posts.

## 🛠 Tools and Resources
- **Textbook**: *Modern Systems Analysis and Design* by Valacich & George (10th Edition)
- **Modeling Tools**: UML diagrams, Gantt charts, object models
- **Communication Tools**: Technical writing and presentation strategies

## Portfolio Reflection
1. DriverPass Project Summary
The DriverPass project involved designing an Online Training and Management System for the client, DriverPass (Liam). The core purpose was to professionalize and scale their business by providing structured training to students preparing for their DMV driving tests.

The requested system was a cloud-based web application with a relational database. It needed three primary user interfaces—a Student Portal, an Instructor/Driver Module, and a Secretary/Admin Interface. The system's main functions were to allow customers to schedule and pay for two-hour on-the-road lessons, take online classes and practice tests, and manage core business operations like driver assignments, vehicle tracking, and activity reporting. The ultimate goal was to reduce the high failure rate at the DMV by improving student preparedness.

2. What did you do particularly well?
I believe I excelled in the system modeling and security requirements definition.

System Modeling (UML Diagrams): The UML diagrams, particularly the Class Diagram and Use Case Diagram, clearly mapped the complex business logic. The Class Diagram established the necessary many-to-many relationships between key entities like Student, Driver, Car, and Reservation, which is crucial for the system's core scheduling and reporting functionality.

Security and Accountability: I thoroughly addressed the non-functional requirements for security. The design includes role-based security for distinct user access levels (Owner, IT, Secretary, Driver, Customer) and implements an Activity Logging component to track and attribute all user actions (reservations, cancellations, modifications) for accountability.

3. If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
I would choose to revise the UML Activity Diagram for the "Schedule Driving Lesson" use case.

The current diagram shows an activity labeled "Redirect to Payment Gateway" if the slot is not available. This is a logical error. A payment step should only occur after a slot has been checked and confirmed as available.

Improvement: I would revise the diagram so the flow from the "Is Slot Available?" decision point goes:

NO: Returns an error message or redirects the user to select another date/time.

YES: Proceeds to the payment gateway before finally updating the reservation record. This ensures that the system only processes payment for a confirmed, available reservation slot.

4. How did you interpret the user’s needs and implement them into your system design? Why is it so important to consider the user’s needs when designing?
I interpreted the users' needs by first defining the various user roles (Student, Driver, Secretary, Admin) and then assigning specific interfaces and functional requirements to each one.

Interpretation and Implementation:

The Student's need for flexible learning and booking led to the design of a responsive web-based interface with a clear online test interface and scheduling calendar.

The Secretary's need for efficiency in phone/office bookings was addressed by designing a dedicated input form for efficient customer registration and scheduling.

The Driver's need for record-keeping resulted in a system component that allows them to log lesson times (Start/End Hour) and Driver Comments.

Importance of User Needs: Considering user needs is critical because it directly dictates system adoption and project success. If the system is not usable (e.g., the scheduling is too complicated for a Student) or functional for key employees (e.g., the Driver can't easily log a lesson), it won't be used correctly, and the business goals (like reducing the high failure rate) will not be met. Designing for the user ensures usability, accessibility, and client satisfaction.

5. How do you approach designing software? What techniques or strategies would you use in the future to analyze and design a system?
My approach to software design is requirements-driven and model-based. I begin by clearly defining the business and functional requirements (Project One) , which then serve as the foundation for the system design (Project Two).

Analysis: Identify the core problem, stakeholders, and business goals.

Requirements Elicitation: Define the necessary Functional Requirements (what the system must do) and Nonfunctional Requirements (constraints like security and performance).

Modeling: Translate requirements into visual models using UML (Use Case, Activity, Sequence, Class Diagrams) to conceptualize the architecture, user interactions, and data structure.

Technical Design: Specify the necessary infrastructure, software, and security protocols to implement the models.

## 👨‍🏫 Instructor Collaboration
This repository is part of my computer science portfolio. My instructor has been added as a collaborator to review progress and provide feedback.

## 📌 Note
This repository is intended for academic use and showcases my learning and development in system analysis and design. All content adheres to SNHU’s academic integrity and copyright policies.

Getting Started To explore the code in this repository, you can clone it to your local machine using the following command:

git clone https://github.com/ShAd0w-R3BeL/CS-250.git

Each project's folder will contain a README file with specific instructions on how to compile and run the code.

Contact Feel free to reach out to me with any questions or feedback.

Name: Matthew Wood

Email: matthew.wood16@snhu.edu

LinkedIn: https://www.linkedin.com/in/matthew-r-wood-56b3b44b/
