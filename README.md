# Task-3
Task 2: Cloud Storage File Manager using AWS S3
Objective
The objective of this task is to use Amazon S3 (Simple Storage Service) as cloud storage and create a Python application that can upload, download, list, and delete files from an S3 bucket using the Boto3 library.
Tools and Technologies Used
Amazon Web Services (AWS)
Amazon S3
Python 3
Boto3 Library
AWS CLI
Visual Studio Code
Process
Step 1: Create an S3 Bucket
Log in to the AWS Management Console.
Open the Amazon S3 service.
Click Create Bucket.
Enter a unique bucket name (e.g., mohini-files-bucket).
Select the desired AWS Region.
Keep the default settings (or configure permissions as required).
Click Create Bucket.
Output: A new S3 bucket is created successfully.
Step 2: Configure AWS Credentials
Create an IAM user with permission to access Amazon S3.
Generate an Access Key ID and Secret Access Key.
Open the terminal and configure AWS CLI:
aws configure
Enter:
Access Key ID
Secret Access Key
Region (e.g., ap-south-1)
Output format (json)
Output: AWS CLI is configured and ready to access S3.
Step 3: Create the Python Project
Create a project folder containing:
S3_File_Manager/
│── upload.py
│── download.py
│── list_files.py
│── delete.py
└── requirements.txt
Install the required library:
pip install boto3
Step 4: Upload a File
Run the upload script:
python upload.py
The program uploads a local file to the S3 bucket.
Expected Output:
sample.txt uploaded successfully.
In the screenshot, you can see the uploaded files listed inside the S3 bucket.
Step 5: List Files
Run:
python list_files.py
The script retrieves and displays all files stored in the S3 bucket.
Expected Output:
sample.txt
my-notes.txt
image.png
This confirms that the files are successfully stored in Amazon S3.
Step 6: Download a File
Run:
python download.py
The selected file is downloaded from the S3 bucket to the local system.
Expected Output:
sample.txt downloaded successfully.
The downloaded file appears in the project folder.
Step 7: Delete a File
Run:
python delete.py
The specified file is removed from the S3 bucket.
Expected Output:
my-notes.txt deleted successfully.
The S3 bucket now contains one less file, as shown in the screenshot.
Testing
The application was tested by:
Uploading a file to Amazon S3.
Listing all files stored in the bucket.
Downloading a file from the bucket.
Deleting a file from the bucket.
Verifying each operation through both the terminal output and the AWS S3 Console.
Result
The Cloud Storage File Manager was successfully implemented using Python, Boto3, and Amazon S3. The application can upload, list, download, and delete files programmatically, demonstrating how cloud storage operations can be automated using AWS services. This task provides practical
