# BookAResource
Abstract

Created a simple serverless web application that enables users to search for a book, add and
issue a book in the library. The application will present users with an HTML based user
interface for searching the book if available in the library and to register any new book to the
library and will interface on the backend with a RESTful web service to submit the request.
The application will also provide facilities for users to register for the service and log in before
utilising the services.

Prerequisite

To complete this project, utilised an AWS account, an account with AWS free tier to
add mapping to your app, a text editor, and a web browser.

Application Architecture

The application architecture uses AWS Lambda, Amazon API Gateway, Amazon
DynamoDB, Amazon Cognito, and AWS Amplify Console. Amplify Console provides
continuous deployment and hosting of the static web resources including HTML, CSS,
JavaScript, and image files which are loaded in the user's browser. JavaScript executed in the
browser sends and receives data from a public backend API built using Lambda and API
Gateway. Amazon Cognito provides user management and authentication functions to secure
the backend API. Finally, DynamoDB provides a persistence layer where data can be stored by
the API's Lambda function.

Technologies Used:
1. Amazon S3 bucket: It is used for storing files and hosting a static website by generating
a public bucket policy.
2. AWS Lambda: It is used for implementing business logic methods. Here for getting
book details from dynamo DB and for registering new book details to dynamo DB
3. Amazon API Gateway: Amazon API Gateway is a fully managed service that makes
it easy for developers to create, publish, maintain, monitor, and secure APIs at any
scale. APIs act as the "front door" for applications to access data, business logic, or
functionality from your backend services. Here we used REST API type for
implementing GET and POST methods
4. AWS IAM Roles: Two different roles were created for both GET and POST API
Gateway Lambda functions for red, write access to dynamo db.
5. Amazon Dynamo DB: Amazon DynamoDB is a fully managed, serverless, key-value
NoSQL database designed to run high-performance applications at any scale.
DynamoDB offers built-in security, continuous backups, automated multi-Region
replication, in-memory caching, and data import and export tools. It is used to create
dynamo DB Book Details table for storing and displaying the book details.
6. Postman: The Postman platform includes a comprehensive set of tools that help
accelerate the API lifecycle—from design, testing, documentation, and mocking to the
sharing and discoverability of APIs.
7. HTML: To create login, registration, search, add and issue a book page
8. CSS: To provide styling to all the pages
9. JavaScript: To implement AJAX functions for GET and POST methods interaction
with API Gateway and Lambda functions
10. jQuery, AJAX, GitHub tool
    
PROCESS:

1. Static Web Hosting: All static web content including HTML, CSS, JavaScript, images, and
other files will be managed by AWS Amplify Console. End users will then access your site
using the public website URL exposed by AWS Amplify Console. There is no need to run any
web servers or use other services to make your site available.
User Management: Amazon Cognito provides user management and authentication functions
to secure the backend API.
2. Serverless Backend: Amazon DynamoDB provides a persistence layer where data can be
stored by the API's Lambda function.
RESTful API: JavaScript executed in the browser sends and receives data from a public
backend API built using Lambda and API Gateway.

Project Budget

Each service used in this architecture is eligible for the AWS Free Tier. If you are outside the
usage limits of the Free Tier, completing this tutorial will cost you less than $0.25*
