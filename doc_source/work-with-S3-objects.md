# Working with Amazon S3 Objects by Using the AWS Toolkit for JetBrains<a name="work-with-S3-objects"></a>

Objects are the fundamental entities stored in Amazon S3\. Objects consist of object data and metadata\.

**Topics**
+ [Viewing an Object in an Amazon S3 Bucket](#viewing-s3-object-in-bucket)
+ [Opening an Object in the IDE](#opening-s3-object-in-IDE)
+ [Uploading an Object](#uploading-s3-object)
+ [Downloading an Object](#downloading-s3-object)
+ [Deleting an Object](#deleting-s3-object)

## Viewing an Object in an Amazon S3 Bucket<a name="viewing-s3-object-in-bucket"></a>

This procedure opens the **S3 Bucket Viewer**, which can be used to view, upload, download, and delete objects grouped by folders in an Amazon S3 bucket\.

1. [Open AWS Explorer](key-tasks.md#key-tasks-open-explorer), if it isn't already open\.

1. To view a bucket's objects, do either of the following:
   + Double\-click the name of the bucket\.
   + Right\-click the name of the bucket and select **View Bucket**\.

The **S3 Bucket Viewer** displays information about the bucket's name, [Amazon Resource Name \(ARN\)](https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html), and creation date\. The objects and folders in the bucket are available in the pane beneath\.

## Opening an Object in the IDE<a name="opening-s3-object-in-IDE"></a>

If the object in an Amazon S3 bucket is a file type recognized by the IDE, you can download a read\-only copy and open it in the IDE\.

1. To find an object to download, open the **S3 Bucket Viewer** \(see [Viewing an Object in an Amazon S3 Bucket](#viewing-s3-object-in-bucket)\)\.

1. Double\-click the name of the object\.

The file opens in the default IDE window for that file type\.

## Uploading an Object<a name="uploading-s3-object"></a>

1. To find the folder you want to upload objects to, open the **S3 Bucket Viewer** \(see [Viewing an Object in an Amazon S3 Bucket](#viewing-s3-object-in-bucket)\)\.

1. Right\-click the folder and select **Upload**\.

1. In the dialog box, select the files you want to upload\.
**Note**  
You can upload multiple files at once\. You cannot upload directories\.

1. Click **OK**\.

## Downloading an Object<a name="downloading-s3-object"></a>

1. To find a folder to download objects from, open the **S3 Bucket Viewer** \(see [Viewing an Object in an Amazon S3 Bucket](#viewing-s3-object-in-bucket)\)\.

1. Click a folder to display its objects\.

1. Right\-click an object and select **Download\.\.\.**\.

1. In the dialog box, select the download location\.

1. Select **OK**\.
**Note**  
If a file already exists in the download location, you can overwrite it or leave it in place by skipping the download\.

## Deleting an Object<a name="deleting-s3-object"></a>

1. To find the object to delete, open the **S3 Bucket Viewer** \(see [Viewing an Object in an Amazon S3 Bucket](#viewing-s3-object-in-bucket)\)\.

1. After you select the object, delete it by either
   + Pressing the **Delete** key\.
   + Right\-clicking and selecting **Delete**\.
**Note**  
You can select and delete multiple objects at once\.

1. To confirm the deletion, select **Delete**\.