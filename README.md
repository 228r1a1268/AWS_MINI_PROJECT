# AWS_MINI_PROJECT
*Log Aggregation and Monitoring using AWS CloudWatch Logs*

This mini project focuses on designing a real-time, serverless log aggregation and analysis system using AWS. The objective is to collect logs from different sources, analyze them centrally using CloudWatch Logs, and generate alerts for critical events through Amazon SNS.

To simulate real-world application logging, a simple frontend quiz app is integrated with AWS Lambda functions that handle login, signup, quiz generation, and score submission. Logs from both Lambda and a Windows EC2 instance are routed to CloudWatch Log Groups and monitored with metric filters and alarms.


 🎯 Objectives

- Collect system and application logs from EC2 and Lambda
- Centralize log storage and analysis using CloudWatch
- Create metric filters and alarms to monitor important log events
- Use SNS for real-time alert notifications
- Demonstrate end-to-end monitoring using a quiz-based frontend


🧰 Technologies Used

- *AWS Lambda*– Backend for login/signup/quiz APIs
- *Amazon EC2 (Windows)* – Source of system logs
- *Amazon CloudWatch Logs* – Central log aggregation
- *Amazon CloudWatch Alarms* – Alerting on log conditions
- *Amazon SNS* – Email alerts for failures
- *Amazon DynamoDB* – Data storage (users & quiz results)
- *API Gateway* – HTTP interface for Lambda
- *HTML/CSS/JavaScript* – Frontend quiz app



 📁 Project Structure

AWS_MINI_PROJECT/
├── backend/
│ ├── signup_lambda.py
│ ├── login_lambda.py
│ ├── get_quiz_lambda.py
│ └── submit_quiz_lambda.py
├── frontend/
│ ├── signup.html
│ ├── login.html
│ ├── quiz.html
│ └── style.css
├── README.md
└── project_report.pdf



🚀 Execution Flow

1. EC2 instance streams logs to CloudWatch using the CloudWatch Agent.
2. Lambda functions triggered via API Gateway handle frontend requests.
3. All activity is logged and sent to CloudWatch Log Groups.
4. Metric filters analyze the logs in real time.
5. Alarms are configured to trigger SNS notifications (email) based on certain log patterns.
6. Quiz scores and user data are stored in DynamoDB for persistence.



*Output Highlights*

- Verified logs in CloudWatch from both EC2 and Lambda
- Triggered SNS email alerts on alarm thresholds
- Frontend displayed a working 3-question quiz with login and signup
- Data successfully stored and queried from DynamoDB


👨‍💻 Author

Avinash Vishwakarma  
Reg. No: 228R1A1268  
CMR Engineering College, Hyderabad  
B.Tech – Information Technology (2022–2026)
