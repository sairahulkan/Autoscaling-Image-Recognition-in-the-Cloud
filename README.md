Overview
This project demonstrates the development of a scalable face recognition system deployed on AWS. By leveraging EC2, SQS, S3, IAM, and Python, the system is designed to handle high volumes of requests efficiently. Custom auto-scaling is implemented to manage 200 requests within 120 seconds, and web server performance is optimized using Redis caching and AWS CloudWatch.

Features
Scalable Face Recognition: Deployed on EC2 instances, decoupled frontend and backend using SQS.
Custom Auto-Scaling: Handles 200 requests in under 120 seconds.
Data Persistence: Utilizes S3 for storing and retrieving data.
Performance Optimization: Web server performance improved with Redis caching, reducing data retrieval times by 60%.
Monitoring and Incident Resolution: AWS CloudWatch for efficient monitoring and decreased incident resolution times.
Technologies Used
AWS EC2: Compute capacity in the cloud.
AWS S3: Scalable storage solution.
AWS SQS: Queue service for decoupling components.
AWS IAM: Securely manage access to AWS services.
Redis: In-memory data structure store for caching.
AWS CloudWatch: Monitoring and logging.
Python: Programming language used for implementation.
Installation and Setup
Prerequisites
AWS Account
AWS CLI configured
Python 3.x
Redis