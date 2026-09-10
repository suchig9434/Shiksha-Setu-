🎓 Shiksha Setu
Smart Academic Assignment, CT & Submission Management System

“Bridging the gap between teachers and students through smart academic automation.”

Shiksha Setu is a full-stack academic management platform designed to digitize and simplify the process of assignment, CT (Class Test), academic task distribution, submission, evaluation, feedback, and notification.

The platform provides a centralized environment where teachers can create and manage academic tasks, while students can access, submit, track, and receive feedback on their work digitally.

The primary goal is to eliminate unnecessary paperwork, reduce manual tracking, improve transparency, and make everyday academic communication faster and more reliable.

📌 Table of Contents
Overview
Problem Statement
Proposed Solution
Objectives
Key Features
User Roles
System Workflow
System Architecture
Modules
Database Design
Technology Stack
Security
Notification System
Submission Management
Analytics
API Design
Project Structure
Installation
Future Scope
Real-World Impact
Learning Outcomes
Conclusion
🔎 Overview

In many colleges, assignment and CT submissions are still handled through traditional methods.

Students may have to:

Print assignments
Prepare physical copies
Visit faculty cabins
Wait for teachers
Manually confirm whether an assignment was received
Keep track of multiple deadlines

At the same time, teachers have to:

Collect assignments
Maintain submission records
Identify students who have not submitted
Manage files
Track late submissions
Evaluate assignments
Communicate marks and feedback

This creates unnecessary effort for both students and faculty.

Shiksha Setu provides a digital solution.

Instead of:

Student
   ↓
Prepare Assignment
   ↓
Print Assignment
   ↓
Find Faculty
   ↓
Visit Cabin
   ↓
Submit
   ↓
Wait for Confirmation

The process becomes:

Student
   ↓
Login to Shiksha Setu
   ↓
Open Assignment
   ↓
Upload Solution
   ↓
Click Submit
   ↓
Instant Confirmation
   ↓
Teacher Notification
   ↓
Evaluation
   ↓
Marks + Feedback
🚨 Problem Statement

The traditional academic submission process has several challenges:

For Students
Physical submission is inconvenient
Students may need to visit faculty cabins
Submission status may not be immediately known
Deadlines can be missed
Multiple assignments are difficult to track
Feedback is not centralized
For Teachers
Manual record maintenance
Large number of files to manage
Difficulty identifying pending students
Manual communication
Difficult tracking of late submissions
Time-consuming evaluation management
For Institutions
Paper consumption
Lack of centralized records
Limited academic analytics
Non-standardized submission process
💡 Proposed Solution

Shiksha Setu provides a centralized digital platform that connects teachers and students.

Teacher
Login
  ↓
Create Assignment / CT
  ↓
Set Deadline
  ↓
Add Instructions
  ↓
Publish
Student
Login
  ↓
View Assignment
  ↓
Read Instructions
  ↓
Upload Solution
  ↓
Submit
System
Validate Submission
        ↓
Store Metadata
        ↓
Store File
        ↓
Generate Submission ID
        ↓
Send Notifications
Teacher
View Submission
       ↓
Evaluate
       ↓
Add Marks
       ↓
Add Feedback
Student
Receive Result
       ↓
View Marks
       ↓
Read Feedback
🎯 Objectives

The major objectives of Shiksha Setu are:

Digitize assignment and CT submission.
Reduce dependency on physical submissions.
Minimize paperwork.
Provide centralized academic task management.
Automate submission notifications.
Track deadlines and late submissions.
Provide transparent submission status.
Simplify teacher evaluation.
Provide students with marks and feedback.
Generate useful academic submission analytics.
✨ Key Features
👨‍🏫 Teacher Features
Authentication

Teachers can securely log into their accounts.

Assignment Creation

Teachers can create:

Assignments
CT tasks
Practical tasks
Projects
Class activities

Each task can contain:

Title
Description
Subject
Instructions
Maximum Marks
Start Date
Deadline
Reference Material
Submission Management

Teachers can view:

Submitted assignments
Pending assignments
Late submissions
Checked assignments
Unchecked assignments
Evaluation

Teachers can:

Open submissions
Download files
Assign marks
Add feedback
Mark submissions as evaluated
👨‍🎓 Student Features

Students can:

Register/login
View assigned subjects
View assignments
View CT tasks
Read instructions
Download resources
Check deadlines
Upload solutions
Submit assignments
Receive confirmation
Track submission status
View marks
View feedback
🔔 Smart Notification System

Shiksha Setu includes automated email notifications.

Assignment Created
Teacher creates assignment
          ↓
Assignment published
          ↓
Students notified
Assignment Submitted
Student submits
       ↓
System verifies
       ↓
Teacher receives email
       ↓
Student receives confirmation
Assignment Evaluated
Teacher adds marks
       ↓
Evaluation saved
       ↓
Student notified
       ↓
Marks + feedback available
⏰ Deadline Management

Every assignment has a deadline.

The system automatically determines whether a submission is:

Upcoming
   ↓
Active
   ↓
Submitted
   ↓
Evaluated

If the deadline has passed:

Student submits
       ↓
Deadline Check
       ↓
Past Deadline?
    /       \
  YES        NO
   ↓          ↓
 LATE       ON TIME

This makes late submissions easy to identify.

📤 Digital File Submission

Students can upload assignment files directly.

The system validates:

File type
File size
Student identity
Assignment identity
Submission deadline

Supported formats can include:

PDF
DOC
DOCX
PPT
PPTX
ZIP
Images

Each submission is associated with a unique record.

Example:

Submission ID:
SS-DBMS-2026-00124
🆔 Submission Tracking

Every submission maintains complete metadata:

Submission ID
Student ID
Student Name
Assignment ID
Assignment Name
File Name
Submission Date
Submission Time
Status
Late Status
Evaluation Status
Marks
Feedback

This provides a reliable digital audit trail.

📊 Academic Analytics

The teacher dashboard can provide real-time statistics.

Example:

--------------------------------
      ASSIGNMENT ANALYTICS
--------------------------------

Total Students        60

Submitted             51
Pending                9
Late                   4
Checked               43

Submission Rate       85%
Average Marks         8.2/10
--------------------------------

Teachers can identify students who have not submitted and monitor overall class participation.

🔎 Search & Filtering

Teachers can filter submissions by:

Student
Assignment
Subject
Submission status
Evaluation status
Late status
Submission date

This becomes especially useful when a teacher manages multiple classes.

🔐 Security Architecture

Security is an important part of Shiksha Setu.

The system can implement:

Authentication
Secure login
Password hashing
JWT authentication
Authorization

Role-based access:

ADMIN
TEACHER
STUDENT
API Security

Protected endpoints ensure that:

Students cannot access teacher dashboards
Students cannot modify other students' submissions
Teachers cannot modify unauthorized resources
Only authorized users can access academic data
File Security
File type validation
File size validation
Secure file storage
Ownership verification
👥 User Roles
Student
Student
 ├── Login
 ├── View Subjects
 ├── View Assignments
 ├── Download Resources
 ├── Upload Solution
 ├── Submit
 ├── Track Status
 ├── View Marks
 └── View Feedback
Teacher
Teacher
 ├── Login
 ├── Manage Subjects
 ├── Create Assignment
 ├── Create CT
 ├── Set Deadline
 ├── View Submissions
 ├── Download Files
 ├── Evaluate
 ├── Add Marks
 └── Add Feedback
Admin
Admin
 ├── Manage Students
 ├── Manage Teachers
 ├── Manage Subjects
 ├── Manage Courses
 └── Monitor Platform
🔄 Complete System Workflow
                    SHIKSHA SETU
                         │
              ┌──────────┴──────────┐
              │                     │
           TEACHER                STUDENT
              │                     │
              ▼                     ▼
        Create Task            Login
              │                     │
              ▼                     ▼
       Set Deadline          View Assignment
              │                     │
              ▼                     ▼
          Publish              Upload File
              │                     │
              └──────────┬──────────┘
                         ▼
                  Submission
                    Validation
                         │
                         ▼
                   File Storage
                         │
                         ▼
                Database Record
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
         Teacher Email        Student Email
              │                     │
              ▼                     ▼
          Evaluation          Confirmation
              │
              ▼
        Marks + Feedback
              │
              ▼
       Student Notification
🏗️ System Architecture
┌────────────────────────────────────────────┐
│              USER INTERFACE                │
│                                            │
│       React + TypeScript + Tailwind        │
└─────────────────────┬──────────────────────┘
                      │
                      │ REST API
                      ▼
┌────────────────────────────────────────────┐
│             BACKEND SERVER                 │
│                                            │
│              Spring Boot                  │
│                                            │
│  Authentication │ Assignment │ Submission │
│  Evaluation     │ Notification │ Analytics │
└─────────────┬──────────┬──────────┬────────┘
              │          │          │
              ▼          ▼          ▼
          ┌───────┐  ┌────────┐  ┌──────────┐
          │ MySQL │  │ File   │  │ Email    │
          │       │  │Storage │  │ Service  │
          └───────┘  └────────┘  └──────────┘
🗄️ Database Design

Core entities include:

User
Student
Teacher
Admin
Subject
Assignment
Submission
Evaluation
Notification
Relationship
Teacher
   │
   │ creates
   ▼
Assignment
   │
   │ receives
   ▼
Submission
   │
   │ evaluated by
   ▼
Evaluation
   │
   ├── Marks
   └── Feedback
Important Database Relationships
One Teacher
     │
     └──────► Many Assignments

One Assignment
     │
     └──────► Many Submissions

One Student
     │
     └──────► Many Submissions

One Submission
     │
     └──────► One Evaluation
🛠️ Technology Stack
Frontend
React.js
TypeScript
HTML5
CSS3
Tailwind CSS
Axios
Backend
Java
Spring Boot
Spring Security
RESTful APIs
JWT
Database
MySQL
JPA
Hibernate
File Storage
Cloudinary / AWS S3
Email
SMTP
JavaMail
Development Tools
Git
GitHub
Postman
IntelliJ IDEA
VS Code
🔌 REST API Design

Example API structure:

Authentication
POST /api/auth/register
POST /api/auth/login
POST /api/auth/logout
Assignments
POST   /api/assignments
GET    /api/assignments
GET    /api/assignments/{id}
PUT    /api/assignments/{id}
DELETE /api/assignments/{id}
Submissions
POST /api/submissions
GET  /api/submissions/{id}
GET  /api/assignments/{id}/submissions
Evaluation
POST /api/evaluations
PUT  /api/evaluations/{id}
GET  /api/submissions/{id}/evaluation
Notifications
GET /api/notifications
PUT /api/notifications/{id}/read
📁 Project Structure
Shiksha-Setu/
│
├── frontend/
│   │
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── services/
│   │   ├── hooks/
│   │   ├── context/
│   │   ├── utils/
│   │   └── App.tsx
│   │
│   ├── package.json
│   └── README.md
│
├── backend/
│   │
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/shikshasetu/
│   │       │       ├── controller/
│   │       │       ├── service/
│   │       │       ├── repository/
│   │       │       ├── entity/
│   │       │       ├── dto/
│   │       │       ├── security/
│   │       │       └── exception/
│   │       │
│   │       └── resources/
│   │           └── application.properties
│   │
│   └── pom.xml
│
├── database/
│   ├── schema.sql
│   └── sample-data.sql
│
├── docs/
│   ├── architecture.md
│   ├── api-documentation.md
│   └── database-design.md
│
├── screenshots/
│
├── .gitignore
└── README.md
⚙️ Installation & Setup
1. Clone Repository
git clone https://github.com/yourusername/shiksha-setu.git
2. Navigate to Project
cd shiksha-setu
3. Setup Database

Create a MySQL database:

CREATE DATABASE shiksha_setu;

Update database credentials inside:

application.properties
4. Start Backend
cd backend
mvn spring-boot:run
5. Start Frontend
cd frontend
npm install
npm run dev
🧪 Testing

The application can be tested using:

Postman
JUnit
Mockito
Browser testing
API integration testing

Testing areas include:

Authentication
Authorization
Assignment Creation
File Upload
Submission
Deadline Validation
Email Notification
Evaluation
Database Operations
🚀 Future Scope

Shiksha Setu can evolve into a complete Digital Academic Management Ecosystem.

🤖 AI Integration

Future versions can include:

AI-powered plagiarism detection
Duplicate submission detection
AI-generated assignment summaries
Automated feedback suggestions
Assignment difficulty analysis
Student performance prediction
📱 Mobile Application

Android/iOS application for:

Assignment notifications
Mobile submissions
Teacher evaluation
Push notifications
📅 Academic Calendar

Integrate:

Assignments
CTs
Exams
Practical submissions
Events
Holidays
📊 Advanced Analytics

Future dashboards can provide:

Student performance trends
Subject-wise performance
Assignment completion rate
Late submission trends
Class-level analytics
🏫 Institution-Level Deployment

The platform can be expanded to support:

College
   ↓
Department
   ↓
Course
   ↓
Semester
   ↓
Subject
   ↓
Teacher
   ↓
Student

This makes the system scalable for an entire institution.

🌍 Real-World Impact
👨‍🎓 Students
Save time
No unnecessary cabin visits
Easy submission
Instant confirmation
Centralized deadlines
Easy access to feedback
👨‍🏫 Teachers
Less paperwork
Centralized submissions
Automated notifications
Easy evaluation
Better tracking
Useful analytics
🏫 Institutions
Digital academic workflow
Reduced paper usage
Centralized records
Better transparency
Scalable infrastructure
💼 Why This Project Is Valuable

Shiksha Setu demonstrates practical software engineering concepts rather than being only a basic academic CRUD application.

The project involves:

Frontend Development
        +
Backend Development
        +
REST API Design
        +
Database Management
        +
Authentication
        +
Authorization
        +
File Upload
        +
Cloud Storage
        +
Email Automation
        +
Deadline Processing
        +
Evaluation System
        +
Analytics

Therefore, it provides experience in building a real-world, multi-user software system.

🧠 Learning Outcomes

Through this project, developers can learn:

Software Development
Full-stack application development
MVC architecture
REST API development
Client-server communication
Backend
Spring Boot
Spring Security
JWT
JPA/Hibernate
Exception handling
API validation
Database
Relational database design
Entity relationships
SQL queries
Database normalization
Frontend
React components
State management
API integration
Responsive UI
Form validation
DevOps & Tools
Git
GitHub
API testing
Environment configuration
Deployment
📈 Project Roadmap
Phase 1
├── Project Setup
├── Database Design
└── UI Design

Phase 2
├── Authentication
├── Student Module
└── Teacher Module

Phase 3
├── Assignment Management
├── File Upload
└── Submission System

Phase 4
├── Email Notifications
├── Deadline Management
└── Evaluation System

Phase 5
├── Analytics Dashboard
├── Security Improvements
└── Testing

Phase 6
├── Deployment
├── Documentation
└── AI Features
⭐ Project Vision

The long-term vision of Shiksha Setu is to become a unified digital bridge between students, teachers, and educational institutions.

Instead of treating assignment submission as a simple file-upload process, Shiksha Setu aims to create a complete academic workflow:

CREATE
   ↓
DISTRIBUTE
   ↓
SUBMIT
   ↓
TRACK
   ↓
EVALUATE
   ↓
FEEDBACK
   ↓
ANALYZE
🏆 Conclusion

Shiksha Setu is a smart academic submission and management platform designed to solve a common problem faced by students and teachers in colleges.

By replacing manual assignment submission with a centralized digital workflow, the platform improves:

Efficiency • Transparency • Accessibility • Communication • Record Management

The project combines modern full-stack technologies with real-world academic requirements to create a scalable and practical software solution.

Shiksha Setu — A Digital Bridge Between Teachers and Students.
👩‍💻 Developer

Suchi Goel

B.Tech Computer Science & Engineering

Areas of Interest

Java Python C++ TypeScript React Spring Boot MySQL AI/ML Data Analytics

⭐ Support

If you find Shiksha Setu useful or interesting, consider giving this repository a ⭐.

Contributions, suggestions, and feedback are welcome.

Built with ❤️ to solve
