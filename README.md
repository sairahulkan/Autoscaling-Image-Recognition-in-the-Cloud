# Autoscaling Image Recognition Application in the Cloud

## Overview
This project demonstrates the development of a scalable face recognition system deployed on AWS. By leveraging EC2, SQS, S3, IAM, and Python, the system is designed to handle high volumes of requests efficiently. Custom auto-scaling is implemented to manage 200 requests within 120 seconds, and web server performance is optimized using Redis caching and AWS CloudWatch.

## Features
- **Scalable Face Recognition**: Deployed on EC2 instances, decoupled frontend and backend using SQS.
- **Custom Auto-Scaling**: Handles 200 requests in under 120 seconds.
- **Data Persistence**: Utilizes S3 for storing and retrieving data.
- **Performance Optimization**: Web server performance improved with Redis caching, reducing data retrieval times by 60%.
- **Monitoring and Incident Resolution**: AWS CloudWatch for efficient monitoring and decreased incident resolution times.

## Technologies Used
- **AWS EC2**: Compute capacity in the cloud.
- **AWS S3**: Scalable storage solution.
- **AWS SQS**: Queue service for decoupling components.
- **AWS IAM**: Securely manage access to AWS services.
- **Redis**: In-memory data structure store for caching.
- **AWS CloudWatch**: Monitoring and logging.
- **Python**: Programming language used for implementation.

## Installation and Setup

### Prerequisites
- AWS Account
- AWS CLI configured
- Python 3.x
- Redis

### Steps
1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/autoscaling-image-recognition.git
    cd autoscaling-image-recognition
    ```

2. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Setup AWS resources**:
    - **EC2 Instances**: Launch EC2 instances as needed.
    - **S3 Bucket**: Create an S3 bucket for data persistence.
    - **SQS Queue**: Create an SQS queue to decouple frontend and backend.
    - **IAM Roles**: Set up IAM roles and policies for EC2, S3, and SQS access.

4. **Configure Redis**:
    - Install Redis on your server or use a managed Redis service.
    - Update the configuration in the project to point to your Redis instance.

5. **Deploy the application**:
    - Upload your code to EC2 instances.
    - Configure the auto-scaling policies to handle request load.

## Usage
1. **Start the application**:
    ```sh
    python main.py
    ```

2. **Send face recognition requests**:
    - Use the provided API endpoints to send images for recognition.

3. **Monitor performance**:
    - Use AWS CloudWatch to monitor system performance and incidents.

## Performance Optimization
- **Redis Caching**: Significantly reduces data retrieval times during peak usage.
- **AWS CloudWatch**: Helps in monitoring and quick incident resolution.
