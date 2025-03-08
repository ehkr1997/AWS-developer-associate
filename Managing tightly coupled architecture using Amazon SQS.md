# AWS-developer-associate
Managing tightly coupled architecture using Amazon SQS
Course-end Project 1
Description

Use AWS SQS to manage a tightly couple architecture.

 

Description:

In the traditional way of building applications, the applications directly talk to each other. if an application is down, it impacts the other linked applications, and some data might be compromised. This is called tightly coupled architecture.

 

Applications cannot communicate directly with each other. This can be done through AWS SQS, which makes applications highly available. In the below diagram, the Customer Web Applications interacts with the Backend Applications via SQS Queue. For some reason, if the backend applications are down, the Customer Web Application can continue working with the messages being buffered in the SQS Queue. Once the backend application is up, it can start polling the messages from the SQS Queue and update the database. This way, none of the messages are lost, and applications are loosely coupled and not aware of the status of each other.

 

Tools required:

AWS Services: SQS, EC2, IAM, and RDS
