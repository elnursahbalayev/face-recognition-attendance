# Face Recognition Attendance System

A desktop application that uses facial recognition technology to track attendance by allowing users to log in and log out with their faces.

## Features

- **Face Recognition Login/Logout**: Users can log in and log out using their face, which is recognized by the system.
- **User Registration**: New users can register their faces with the system.
- **Attendance Logging**: The system logs attendance with timestamps in a text file.
- **Anti-Spoofing**: Includes protection against photo/video spoofing attempts.
- **User-Friendly GUI**: Simple and intuitive graphical user interface built with tkinter.

## Installation

### Prerequisites

- Python 3.6 or higher
- Webcam

### Steps

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/face-recognition-attendance.git
   cd face-recognition-attendance
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

   Note: Installing `dlib` might require additional setup:
   - On Windows, you'll need Visual Studio with C++ build tools
   - On Linux, you'll need CMake and a C++ compiler

## Usage

1. Run the application:
   ```
   python main.py
   ```

2. The main window will open with your webcam feed and three buttons:
   - **Login**: Click to log your entry time
   - **Logout**: Click to log your exit time
   - **Register New User**: Click to add a new user to the system

3. To register a new user:
   - Click "Register New User"
   - Enter the username in the text field
   - Click "Accept" to save the face data
   - Click "Try Again" to retake the photo

4. Attendance logs are stored in `log.txt` in the format: `username, timestamp, in/out`

## Dependencies

The project relies on the following Python libraries:
- cmake (3.17.2)
- dlib (19.18.0)
- opencv-python (4.6.0.66)
- Pillow (9.2.0)
- face_recognition (1.3.0)

## Project Structure

- `main.py`: Contains the main application code and GUI
- `util.py`: Utility functions for GUI elements and face recognition
- `requirements.txt`: List of required Python packages
- `db/`: Directory where user face data is stored
- `log.txt`: File where attendance logs are stored

## License

[Include license information here]

## Acknowledgements

- This project uses the [face_recognition](https://github.com/ageitgey/face_recognition) library
- GUI built with Python's tkinter