# Smart Attendance Face Recognition System

## Team: YOUR TEAM NAME
- **Team Leader:** ESWARA MANIKANTA CHANDRA PRASAD PERUMALLA
- **Team Members:** Akash B, Agney, Albi Thomson

## Objective
The objective of this project is to automate the process of attendance tracking using a **Face Recognition System**. The system utilizes advanced face detection and recognition techniques to identify and mark attendance in real time. This approach aims to increase efficiency, reduce manual errors, and simplify attendance tracking in institutions and workplaces.

## Problem Statement
Manual attendance marking is prone to errors, time-consuming, and inefficient, especially in large institutions. By leveraging machine learning and computer vision, we aim to create a **Smart Attendance System** that uses face recognition to mark attendance automatically, thus reducing human intervention and enhancing accuracy.

## Proposed Solution
The **Smart Attendance Face Recognition System** recognizes and tracks individuals by identifying their faces from live camera feeds or uploaded images. Once identified, the system automatically marks attendance in a CSV file and sends SMS notifications to absentees.

## Key Skills
- **Programming:** Python
- **Libraries:** OpenCV, Face Recognition, Pandas
- **API Integration:** Twilio for SMS services
- **Machine Learning:** Facial Recognition for identification

## Technologies Used
- **Face Detection and Recognition:** OpenCV, Face Recognition library
- **Data Storage:** CSV for storing attendance data
- **SMS Notification:** Twilio API
- **Image Processing:** Python-based facial encoding and matching

## Approach

### 1. Face Detection and Encoding
The system detects faces from live camera feeds or static images and generates unique encodings for each individual’s face.

<img src="./Images/RA2111003010745.jpg" alt="Face Recognition"/>

### 2. Attendance Marking
Upon successfully recognizing a face, the system marks the individual as present in the attendance CSV file.

<img src="./Resources/Modes/3.png" alt="Attendance Marking" width="300" height="400"/>

### 3. SMS Notification for Absentees
If an individual’s face is not recognized during the attendance marking process, an automated SMS notification is sent to inform them of their absence.


### 4. Database Management
The attendance data is stored in an easy-to-manage CSV file that administrators can access and analyze at any time.

## Project Structure

- **AddDataToDataBase.py:** This script adds users' data and images to the system’s database.
- **EncodeGenerator.py:** Generates facial encodings for each user and saves them in a pickle file.
- **main.py:** The primary script that handles face recognition and attendance marking.
- **sms.py:** Responsible for sending SMS notifications to absent users.
- **keys.py:** Stores sensitive API keys and other configuration details.git init
- **Attendance.csv:** The file where attendance data is stored after being marked by the system.
- **Images Folder:** Contains images of the individuals whose attendance is tracked.

## Insights and Visualizations

- **Face Detection and Recognition Flow:** The system detects faces, encodes them, and matches them with stored encodings to mark attendance.
  

- **Attendance Logs:** All attendance records are stored in a structured CSV file, which can be accessed and reviewed by administrators.
  
  ![Attendance Logs](./Resources/background.png)

## Achievements
- Developed an accurate and efficient **Smart Attendance System** using facial recognition technology.
- Automated the attendance process, reducing the need for manual tracking.
- Implemented SMS notification for absentee tracking.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/smart-attendance-system.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Add images of individuals to the `images/` folder and generate facial encodings:
    ```bash
    python EncodeGenerator.py
    ```

4. Start the face recognition and attendance marking system:
    ```bash
    python main.py
    ```

## Contact
For more information or queries about the project, please contact the team at [pp2549@srmist.edu.in].
