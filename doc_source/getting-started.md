# Getting Started<a name="getting-started"></a>

In this section, we introduce you to the fundamental concepts of a typical Lambda\-based application and the options available to create and test your applications\. In addition, you will be provided with instructions on installing the necessary tools to complete the tutorials included in this guide and create your first Lambda function\. 

## Building Blocks of a Lambda Application<a name="lambda-application-fundamentals"></a>
+ **Function** – A script or program that runs in AWS Lambda\. Lambda passes invocation events to your function\. The function processes an event and returns a response\. For more information, see [Working with Lambda Functions](lambda-introduction-function.md)\.
+ **Runtimes** – Lambda runtimes allow functions in different languages to run in the same base execution environment\. You configure your function to use a runtime that matches your programming language\. The runtime sits in\-between the Lambda service and your function code, relaying invocation events, context information, and responses between the two\. You can use runtimes provided by Lambda, or build your own\. For more infromation, see [AWS Lambda Runtimes](lambda-runtimes.md)\.
+ **Layers** – Lambda layers are a distribution mechanism for libraries, custom runtimes, and other function dependencies\. Layers let you manage your in\-development function code independently from the unchanging code and resources that it uses\. You can configure your function to use layers that you create, layers provided by AWS, or layers from other AWS customers\. For more infromation, see [AWS Lambda Layers](configuration-layers.md)
+ **Event source** – An AWS service, such as Amazon SNS, or a custom service, that triggers your function and executes its logic\. For more information, see [AWS Lambda Event Source Mapping](intro-invocation-modes.md)\.
+ **Downstream resources** – An AWS service, such as DynamoDB tables or Amazon S3 buckets, that your Lambda function calls once it is triggered\. 
+ **Log streams** – While Lambda automatically monitors your function invocations and reports metrics to CloudWatch, you can annotate your function code with custom logging statements that allow you to analyze the execution flow and performance of your Lambda function to ensure it's working properly\.
+ **AWS SAM** – A model to define [serverless applications](https://aws.amazon.com/serverless)\. AWS SAM is natively supported by AWS CloudFormation and defines simplified syntax for expressing serverless resources\. For more information, see [What Is AWS SAM?](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/) in the *AWS Serverless Application Model Developer Guide*\.

## Tools to Create and Test Lambda Functions<a name="lambda-application-tools"></a>

There are three key tools that you use to interact with the AWS Lambda service, described below\. We will cover tools for building AWS Lambda\-based applications in further sections\.
+ **Lambda Console** – Provides a way for you to graphically design your Lambda\-based application, author or update your Lambda function code, and configure event, downstream resources and IAM permissions that your function requires\.
+ **AWS CLI** – A command\-line interface you can use to leverage Lambda's API operations, such as creating functions and mapping event sources\. For a full list of Lambda's API operations, see [Actions](API_Operations.md)\.
+ **AWS SAM CLI** – A command\-line interface you can use to develop, test, and analyze your serverless applications locally before uploading them to the Lambda runtime\. For more information, see [ AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-reference.html#serverless-sam-cli) in the *AWS Serverless Application Model Developer Guide*\.