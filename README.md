# Ethical-Remote-Access-ToolV2
![dark_angel_armor](https://github.com/user-attachments/assets/c93b8c99-978e-4076-b610-efd8cda174b9)

DARKSPACE SOFTWARE AND SECURITY LLC Author: Michael James Blenkinsop (DARK ANGEL)

Table of Contents
Introduction
Features
Supported Platforms
System Requirements
Installation Instructions
Usage Instructions6.1 Instructor Guide (Server)6.2 Student Guide (Client)
Security Considerations
Troubleshooting
Licensing
Contact Information

1. Introduction
The Ethical Remote Access Tool is a secure software solution designed by DARKSPACE SOFTWARE AND SECURITY LLC to facilitate seamless remote access and collaboration between instructors (servers) and students (clients). This tool allows for real-time interaction, screen sharing, group chat, and video conferencing, while ensuring user privacy and security. The system can be easily configured for both LAN and internet use, with options for setting up Dynamic DNS for accessibility beyond local networks.

2. Features
Screen Sharing: Instructors can view multiple students' screens simultaneously.
Video Chat: Supports individual video chat between the instructor and each connected student, with dynamic windows for each session.
Group Chat: Facilitates a group chat feature for real-time text communication among all participants.
Student Details Submission: Students must submit their name, email, and phone number before accessing features.
Notification Email: Instructors can set up email notifications to receive student information when they join the session.
Client-Server Connection: Clients can easily connect to the instructor’s server using an IP address.
Port Reuse for Easy Restarts: The server can reuse the same port immediately after restarting, avoiding typical socket reuse delays.
Dynamic DNS Integration: Added options for DynDNS and NoIP configurations to facilitate easy port forwarding and dynamic IP management.
Cross-Platform Compatibility: Supports Windows, macOS, and Linux, ensuring flexibility for different users.

3. Supported Platforms
The Ethical Remote Access Tool supports the following operating systems:

Windows: Windows 10 and above
macOS: macOS 10.15 (Catalina) and above
Linux: Ubuntu 18.04 and above

The tool requires Python 3.6 or later to function properly.

4. System Requirements
Minimum Requirements:

Processor: Intel i3 or equivalent
RAM: 4 GB
Disk Space: 500 MB available space
Network: Stable internet connection

Recommended Requirements:

Processor: Intel i5 or above
RAM: 8 GB or more
Disk Space: 1 GB available space
Network: High-speed internet connection

5. Installation Instructions
Download and Install Python 3.6 or Later: Ensure Python is installed on your machine.
Install Required Dependencies:Run the following command to install dependencies:
Run the Script:Navigate to the software directory and execute:

6. Usage Instructions
6.1 Instructor Guide (Server)
Launch the Application: Open the remote_access_tool.py script to start the instructor dashboard.
Submit Your Details:Enter your name, email, and phone number.Set up your notification email to receive details of connecting students.
Start Network Server:Click the 'Start Network Server' button to open the server for incoming student connections.
View Student Screens:Use the 'View Screens' button to view connected students' screens in real-time.
Group Chat:Use 'Group Chat' to communicate simultaneously with all connected students.
Video Chat:Use 'Start Video Chat' to initiate individual video chat sessions with each connected student.
Port Forwarding Setup:To enable connectivity over the internet, click on 'Setup DynDNS' or 'Setup NoIP' to configure Dynamic DNS for port forwarding. Visit the respective websites for setup instructions.

6.2 Student Guide (Client)
Launch the Application: Open the remote_access_tool.py script to start the client connection interface.
Connect to Server:Enter the server IP address given by the instructor.Click the 'Connect to Server' button to establish a connection.
Submit Your Details:Fill in your name, email, and phone number to proceed.
Follow Instructor’s Instructions:Once connected, wait for the instructor's instructions to begin screen sharing, group chatting, or participating in video sessions.

7. Security Considerations
Encrypted Communication: All communication between the server and clients occurs over encrypted channels to ensure data privacy.
Mandatory Contact Details: Students are required to submit their contact details before joining any session, which helps maintain accountability.
Email Notifications: Instructors receive emails containing student contact details upon connection, which helps maintain records for safety.

8. Troubleshooting
Common Issues:
Port in Use Error (OSError: [WinError 10048]):Solution: Ensure no other process is using the selected port (5000). Change the port number if necessary and restart the server.
Failed to Connect to Server:Solution: Verify that the server IP address is correct and that the server is actively listening. Ensure the server firewall allows the selected port.
Dependencies Not Installed:Solution: Run the setup script or install dependencies manually using:
