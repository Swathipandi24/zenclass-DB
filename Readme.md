MongoDB Zen Class Program Database

This project is a MongoDB-based database designed for the Zen Class Program. The database contains collections to store data related to users, codekata, attendance, topics, tasks, company drives, and mentors. It also includes queries for retrieving specific information from the database.

 Collections

1. Users
   - Stores information about the students in the Zen class program.
   - Each user has details like `name`, `email`, `codekata_solved`, `attendance`, `tasks_submitted`, and `mentee_of` (mentor information).

2. CodeKata
   - Tracks the number of problems solved by each user in the CodeKata challenge.
   - Fields include `user_id` (references the user), and `problems_solved`.

3. Attendance
   - Stores the attendance records for each user.
   - Fields include `user_id` (references the user), `date`, and `status` (either `present` or `absent`).

4.Topics
   - Stores the topics that are taught in the Zen class program.
   - Each topic has a `name` and a `date` when it was taught.

5. Tasks
   - Stores the tasks assigned to users based on specific topics.
   - Each task has a `name`, `date`, and `topic_id` (references the topic).

6. Company Drives
   - Stores the company placement drives that are held for students.
   - Fields include `company_name`, `drive_date`, and `students_appeared` (array of users who appeared for the drive).

7. Mentors
   - Stores information about the mentors.
   - Fields include `name` and `mentees` (array of users who are mentees of the mentor).

Usage
    Connect to your MongoDB instance using your preferred MongoDB client (e.g., MongoDB Compass, mongo shell).
    Select the appropriate database containing the collections (topics, tasks, company_drives, placements, users, codekata, attendance, mentors).
    Run the provided queries in the MongoDB shell or your client.
