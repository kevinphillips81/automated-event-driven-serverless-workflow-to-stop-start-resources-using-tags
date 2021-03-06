Creating an event-driven, serverless workflow to automate the steps of stopping or starting your resources uses the following services:

- Creating two Amazon EventBridge rules to run on a schedule; one to stop the resources, and the other to start them.

- Using Amazon Simple Notification Service (SNS) to receive Amazon EventBridge rule notifications and pass them on to AWS Lambda functions.

- Writing a stop function, and a start function using AWS Lambda each of which are invoked depending on whether the workflow is to stop the resources, or to start them.


![Start-Stop Neptune Clusters drawio white-bg](https://user-images.githubusercontent.com/52177911/147665436-5117eacf-9d70-40f0-89df-0c740521e84a.png)
