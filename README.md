**FTP Client-Server Application
This project is a simple FTP-like client-server application developed in Python. It supports basic file transfer capabilities, including file upload and download, with a simple authentication mechanism for accessing the server.

**Features
User Authentication: Secure access using a username and password. File Upload: Users can send files to the server. File Download: Users can retrieve files from the server. Clean Exit: Users can cleanly exit the client or server application.

**Prerequisites
Python 3.x installed on both client and server machines.

**Setup Instructions
Server Setup: Place ftp_server.py and users.txt (containing username-password pairs) in the desired directory on the server machine. Client Setup: Place ftp_client.py in the desired directory on the client machine.

**Running the Application
1.Starting the Server Open a terminal and navigate to the server's directory. Start the server by running: python ftp_server.py Replace with your chosen port number.

2.Connecting the Client Open a terminal and navigate to the client's directory. Connect to the server using: python ftp_client.py Replace with the server's IP address and with the port number used when starting the server.

**Usage
After successfully connecting and authenticating, the client can use the following commands:

1.Download a File: get Enter filename to download:

2.Upload a File: upload Enter filename to upload:

3.Exit the Application: exit

**Important Notes
Ensure the users.txt file is placed in the same directory as the server application for authentication purposes. For the get command, ensure the file exists on the server. The server will create a new file prefixed with "new" to avoid overwriting existing files on the client side. For the upload command, ensure the file exists on the client side before attempting to upload.

**Troubleshooting
Authentication Failure: Check the users.txt file on the server for valid username/password combinations. File Upload/Download Issues: Ensure the client and server have permission to read/write to their respective directories.
