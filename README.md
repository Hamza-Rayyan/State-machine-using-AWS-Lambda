# AWS Step Functions Lambda Python  
Creating a sample Python state machine using AWS Lambda and AWS Step Functions.

This state machine basically predicts if the order is billed or failed, have used a general random function to do so.
In this project i have more focused on demonstrate this use of different AWS services like
- IAM Roles
- AWS Lambda Functions 
- AWS Step Functions

Now diving into the project building

* We first need to create a IAM Role with premission policies BasicLambdaFunctions this we will use to create Lambda Function.
Now we create and test Lambda Functions such as Receice-order,Check-stock,order-stock,Delivery-order and BillCustomer for our State Machine
* Each function preform task which you can navigate to that paritculer functions file and explore
* We can open and test them by providing a test case { "Order" : "001" }
* Once all the tests of all the functions are successed.
* we can move to create our state machine using AWS Step Functions
* For this we need to create a seperate IAM role with premission policies Step Function
* Now we can create a State machine in AWS Step function
- we need to write the JSON program for  state machine integrates all the function together with there ARN defined in each functions
- Once our Machine is ready we can start the execution test 
- It may Successed or Fail several time as that depend on a Randam generate Functions
