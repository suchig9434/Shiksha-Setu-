# Shiksha-Setu-

🎓 Shiksha Setu
Smart Academic Assignment & Continuous Assessment Management Platform

Shiksha Setu is a full-stack academic management platform designed to simplify and digitize the process of assignment, CT (Class Test), and academic task distribution and submission between teachers and students.

In many colleges, students still have to submit assignments physically, visit faculty cabins, maintain multiple submission records, and repeatedly ask teachers whether their work has been received. Teachers also spend significant time manually tracking submissions, identifying pending students, checking deadlines, and communicating feedback.

Shiksha Setu solves this problem by providing a centralized digital platform where teachers can create and manage academic tasks, while students can securely submit their work online and receive instant confirmation.

The platform focuses on automation, transparency, accessibility, and efficient academic workflow management.

🚨 Problem Statement

Traditional assignment submission systems often involve:

Physical submission of assignments
Students visiting faculty cabins for submission
Difficulty tracking pending submissions
Lost or misplaced assignments
Manual maintenance of submission records
No centralized deadline tracking
Repeated communication between teachers and students
Difficulty identifying late submissions
Lack of structured feedback and evaluation
Time-consuming submission management for faculty

These problems become more challenging when a teacher handles multiple subjects and hundreds of students.

Shiksha Setu transforms this manual workflow into a centralized, secure and automated digital system.

💡 Proposed Solution

Shiksha Setu provides a single platform where:

Teacher
   │
   ├── Create Assignment / CT
   ├── Add Instructions
   ├── Set Deadline
   ├── Upload Resources
   └── Monitor Submissions
            │
            ▼
       SHIKSHA SETU
            │
            ▼
Student
   │
   ├── View Tasks
   ├── Download Instructions
   ├── Upload Solution
   ├── Submit Digitally
   └── Track Status
            │
            ▼
     Automatic Notification
            │
       ┌────┴────┐
       ▼         ▼
    Teacher    Student
    notified   confirmed

This eliminates unnecessary physical visits and provides a transparent record of every submission.

✨ Key Features
👨‍🏫 Teacher Module

Teachers can:

Securely log in to the platform
Create assignments and CT tasks
Add title, description and instructions
Upload reference material
Set submission deadlines
Specify maximum marks
View all student submissions
Filter students by submission status
Identify pending submissions
Identify late submissions
Download submitted files
Evaluate submissions
Add marks and feedback
Track overall submission statistics
Teacher Dashboard

The dashboard provides important academic insights:

Total Assignments        12
Total Students          120
Submitted                96
Pending                  24
Late Submissions          7
Checked                  82
Average Score           8.4/10
👨‍🎓 Student Module

Students can:

Securely log in
View enrolled subjects
View active assignments
View CT tasks
Read assignment instructions
Download reference files
Check submission deadlines
Upload assignment files
Submit assignments digitally
Receive submission confirmation
Track submission status
View marks
View teacher feedback
Track pending and upcoming tasks
📤 Digital Submission System

Students can upload their assignment files directly through the platform.

Every submission stores important metadata such as:

Student Name
Assignment Name
Submission ID
File Name
Submission Date
Submission Time
Status
Evaluation Status
Marks
Feedback

This creates a reliable digital submission record.

⏰ Smart Deadline Management

Shiksha Setu automatically tracks assignment deadlines.

Submission status can be categorized as:

Upcoming
    ↓
Active
    ↓
Submitted
    ↓
Checked

If a student submits after the deadline:

Submission
     ↓
Deadline Checked
     ↓
Past Deadline?
   /       \
 Yes        No
 ↓          ↓
Late      On Time

This allows teachers to easily identify late submissions.

📧 Automated Email Notifications

One of the major features of Shiksha Setu is automated communication.

When a teacher creates an assignment:

Student receives:

New Assignment Available

When a student submits:

Teacher receives:

New Assignment Submission Received

Student receives:

Assignment Successfully Submitted

When teacher evaluates:

Student receives:

Assignment Evaluated — Marks & Feedback Available

This reduces unnecessary communication and gives both sides confirmation.

🔐 Role-Based Authentication & Authorization

Shiksha Setu uses secure role-based access.

                 Login
                   │
          ┌────────┴────────┐
          │                 │
       Teacher            Student
          │                 │
          ▼                 ▼
 Teacher Dashboard    Student Dashboard

Teachers can access only teacher-specific functionality, while students can access only their academic resources and submissions.

📊 Academic Analytics

Shiksha Setu can provide teachers with useful submission analytics.

Example:
Assignment Submission Analytics

Total Students       60
Submitted            51
Pending               9
Late                  4

Submission Rate      85%
Average Marks       8.2/10

This helps faculty quickly understand student participation and academic activity.

🔎 Submission Tracking

Instead of manually maintaining records, teachers can search and filter submissions.

Possible filters:

Subject
Assignment
Student
Submission status
Late submissions
Evaluation status
Date

This makes handling large classes much easier.

📝 Evaluation & Feedback

Teachers can evaluate submitted assignments directly from the platform.

Example:

Student: Rahul Sharma
Assignment: DBMS Assignment 03

Status: Checked
Marks: 8/10

Feedback:
Good explanation of normalization.
Improve the ER diagram representation.

Students can then view their marks and feedback without visiting the faculty cabin.

🆔 Unique Submission ID

Every successful submission receives a unique submission ID.

Example:

SS-DBMS-2026-000184

This can be used for tracking and verification.

🛡️ Security Features

The platform can implement:

Secure authentication
Password encryption/hashing
JWT-based authentication
Role-based authorization
Protected APIs
Input validation
File type validation
File size restrictions
Secure file storage
Database constraints
Submission ownership verification
🏗️ System Architecture
                    ┌───────────────────┐
                    │      Student      │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌───────────────────┐
                    │   React Frontend  │
                    └─────────┬─────────┘
                              │
                         REST APIs
                              │
                              ▼
                    ┌───────────────────┐
                    │  Spring Boot API  │
                    └─────────┬─────────┘
                              │
              ┌───────────────┼───────────────┐
              ▼               ▼               ▼
        ┌──────────┐    ┌───────────┐   ┌──────────┐
        │  MySQL   │    │ File      │   │ Email    │
        │ Database │    │ Storage   │   │ Service  │
        └──────────┘    └───────────┘   └──────────┘
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
REST APIs
JWT Authentication
Database
MySQL
JPA / Hibernate
File Storage
Cloudinary / AWS S3
Communication
SMTP
JavaMail / Email API
Development Tools
Git
GitHub
Postman
IntelliJ IDEA
VS Code
🗄️ Database Design

Possible core entities:

User
 ├── Student
 └── Teacher

Course
Subject
Assignment
Submission
Evaluation
Notification

Relationship:

Teacher
   │
   ├── creates ──► Assignment
   │                    │
   │                    ▼
   │              Submissions
   │                    │
   │                    ▼
   │               Evaluation
   │                    │
   │                    ▼
   │              Marks + Feedback
   │
   ▼
Notifications
🔄 Complete Workflow
Step 1 — Teacher Login

Teacher securely logs into Shiksha Setu.

Step 2 — Create Academic Task

Teacher creates an assignment or CT task.

Title
Description
Subject
Deadline
Maximum Marks
Reference Material
Step 3 — Students Receive Task

The assignment becomes available on the student dashboard.

Step 4 — Student Uploads Solution

Student uploads the required file.

Step 5 — Submission Validation

System checks:

Authentication
File type
File size
Deadline
Student authorization
Step 6 — Submission Stored

The system stores the submission and generates a unique submission ID.

Step 7 — Notifications

Teacher receives a submission notification.

Student receives confirmation.

Step 8 — Teacher Evaluation

Teacher opens the submission, checks the work and provides marks and feedback.

Step 9 — Student Receives Result

Student can view:

Marks
Feedback
Evaluation Status
🌟 Future Enhancements

Shiksha Setu can be expanded into a complete academic management ecosystem.

🤖 AI-Based Assignment Analysis

AI can help teachers:

Detect duplicate submissions
Identify potential plagiarism
Generate basic submission summaries
Provide preliminary feedback
📱 Mobile Application

Develop Android/iOS applications so students and teachers can manage submissions from mobile devices.

🔔 Push Notifications

Add real-time notifications for:

New assignments
Deadline reminders
Submission confirmation
Marks released
📅 Academic Calendar

Integrate:

Assignment deadlines
CT dates
Exams
Events
Holidays
📈 Advanced Analytics

Provide:

Student performance trends
Subject-wise analytics
Assignment completion rates
Class performance
Late submission patterns
🧑‍💼 Admin Panel

College administrators could manage:

Departments
Teachers
Students
Subjects
Courses
Academic sessions
🎯 Real-World Impact

Shiksha Setu aims to reduce the dependency on physical assignment submission and improve communication between students and faculty.

For Students

✅ No need to visit faculty cabins
✅ Easy digital submission
✅ Submission confirmation
✅ Deadline tracking
✅ Marks and feedback in one place

For Teachers

✅ Centralized submission management
✅ Automatic notifications
✅ Easy tracking of pending students
✅ Faster evaluation workflow
✅ Reduced paperwork

For Institutions

✅ Digital academic workflow
✅ Better record management
✅ Reduced paper usage
✅ Transparent submission tracking
✅ Scalable academic infrastructure

🚀 Why Shiksha Setu?

Shiksha Setu is not just an assignment upload website.

It combines:

Authentication + Role-Based Access + File Management + REST APIs + Database Management + Email Automation + Deadline Tracking + Evaluation + Analytics

to solve a genuine academic workflow problem.

📌 Project Vision

“To create a simple, transparent and technology-driven bridge between teachers and students for everyday academic activities.”

Shiksha Setu — Bridging the gap between classrooms and digital education.

👩‍💻 Developer

Suchi Goel
B.Tech CSE | Java | Python | C++ | AI/ML | Data Analytics

Project Focus

Full-Stack Development • Software Engineering • Academic Automation • Digital Transformation
