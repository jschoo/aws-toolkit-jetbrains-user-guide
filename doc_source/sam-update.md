# Changing \(Updating\) AWS Serverless Application Settings By Using the AWS Toolkit for JetBrains<a name="sam-update"></a>

You must first [deploy the AWS serverless application](key-tasks.md#key-tasks-sam-deploy) that you want to change, if you haven't deployed it already\.
**Note**  
If you want to deploy a serverless application that contains an AWS Lambda function, and you want to deploy that function with any non\-default or optional properties, you must first set those properties in the function's corresponding AWS SAM template file \(for example, in a file named `template.yaml` within the project\)\. For a list of available properties, see [AWS::Serverless::Function](https://github.com/awslabs/serverless-application-model/blob/master/versions/2016-10-31.md#awsserverlessfunction) in the [awslabs/serverless\-application\-model](https://github.com/awslabs/serverless-application-model/) repository on the GitHub website\.

1. With the **Project** tool window already open and displaying the project that contains the serverless application's files, open the project's `template.yaml` file, change the file's contents to reflect the new settings, and then save and close the file\.

1. [Switch to a different AWS Region](key-tasks.md#key-tasks-switch-region) to deploy the serverless application to if necessary\.

1. Right\-click the project's `template.yaml` file, and then choose **Deploy Serverless Application**\.  
![\[Choosing the Deploy Serverless Application command\]](http://docs.aws.amazon.com/toolkit-for-jetbrains/latest/userguide/)

1. Complete the [Deploy Serverless Application dialog](deploy-serverless-application-dialog.md) box, and then choose **Deploy**\. The AWS Toolkit updates the corresponding AWS CloudFormation stack for the deployment\. If the deployment fails, you can try to figure out why by [viewing event logs for the stack](key-tasks.md#key-tasks-cloudformation-logs)\.