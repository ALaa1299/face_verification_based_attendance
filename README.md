# Employee Management System

## Features
- Streamlit web interface for managing employee records
- MongoDB backend with schema validation
- CRUD operations for employee data
- Attendance tracking
- Export attendance records to CSV
- User authentication and role-based access control
- Admin user management interface
- Facial recognition for attendance verification
- Real-time video feed integration

## Setup
1. Install requirements:
pip install streamlit pymongo opencv-python face_recognition deepface --nodeps

2. Make sure MongoDB is running locally.

3. Ensure you have a compatible camera connected to your system for facial recognition.

## Running the Application
Start the Streamlit web interface:
streamlit run employee_ui.py

## Viewing Data

### Web Interface
1. Run the Streamlit app as shown above.
2. Open http://localhost:8501 in your browser.
3. Use the sidebar to navigate through the following sections:
   - Add Employee
   - View Employees
   - Record Attendance
   - Update Employee
   - Delete Employee
   - Export Attendance

### MongoDB Compass
1. Open MongoDB Compass.
2. Connect using:
   - Connection String: mongodb://localhost:27017
   - Database: employee_management
   - Collection: employees

## Database Schema
The database requires these fields for each employee:
- rank (string)
- fullname (string)
- militaryID (integer, unique)
- department (string)
- image_path (string)
- attendance (array, optional)

## Conclusion
This Employee Management System provides a comprehensive solution for managing employee records, attendance tracking, and secure authentication. The integration of facial recognition enhances the attendance verification process, ensuring accuracy and security.

For implementation details or technical questions, please consult the code documentation or contact the development team.
