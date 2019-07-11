# Changing \(Updating\) AWS Lambda Function Settings By Using the AWS Toolkit for JetBrains<a name="lambda-update"></a>

Do one of the following\.
+ With the code file open that contains the [function handler for Java](https://docs.aws.amazon.com/lambda/latest/dg/java-programming-model-handler-types.html) or the [function handler for Python](https://docs.aws.amazon.com/lambda/latest/dg/python-programming-model-handler-types.html), on the main menu, choose **Run, Edit Configurations**\. Complete the [Run/Debug Configurations dialog](run-debug-configurations-dialog.md) box, and then choose **OK**\.
+ [Open the AWS Explorer](key-tasks.md#key-tasks-open-explorer), if it is not already open, [switching to a different AWS Region](key-tasks.md#key-tasks-switch-region) that contains the function if necessary\. Expand **Lambda**, choose the name of the function that you want to change the configuration for, and then do one of the following\.
  + To change settings such as the timeout, memory, environment variables, and execution role: right\-click the name of the function, and then choose **Update Function Configuration**\.  
![\[Choosing the Update Function Configuration command\]](http://docs.aws.amazon.com/toolkit-for-jetbrains/latest/userguide/)

    Complete the [Update Configuration dialog](update-configuration-dialog.md) box, and then choose **Update**\. 
  + To change settings such as the input payload: on the main menu, choose **Run, Edit Configurations**\. Complete the [Run/Debug Configurations dialog](run-debug-configurations-dialog.md) box, and choose **OK**\.  
![\[Choosing the Edit Configurations command\]](http://docs.aws.amazon.com/toolkit-for-jetbrains/latest/userguide/)

    \(If the configuration details are missing, first expand **Templates, AWS Lambda**, and then choose **Local** \(for the local version of the function\) or **Remote** \(for the remote version of that same function\); choose **OK**; and then repeat this procedure from the beginning\.\)
  + To change settings such as the function handler name or Amazon S3 source bucket: right\-click the name of the function, and then choose **Update Function Code**\.  
![\[Choosing the Update Function Code command\]](http://docs.aws.amazon.com/toolkit-for-jetbrains/latest/userguide/)

    Complete the [Update Code dialog](update-code-dialog.md) box, and then choose **Update**\.
  + To change any other available property settings that are not listed in the preceding bullets, change those settings in the function's corresponding AWS SAM template file \(for example, in a file named `template.yaml` within the project\)\. For a list of available property settings, see [AWS::Serverless::Function](https://github.com/awslabs/serverless-application-model/blob/master/versions/2016-10-31.md#awsserverlessfunction) in the [awslabs/serverless\-application\-model](https://github.com/awslabs/serverless-application-model/) repository on the GitHub website\. 