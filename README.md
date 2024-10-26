# Streamlining AWS Policy Development and Implementation for Enhanced Security

![Proj Img](https://imgur.com/2TBqoOJ.jpg) 


## Introduction

This project demonstrates the streamlined process of designing and implementing AWS policies to enhance security and control over AWS services.

### Components used to complete this project:

- Amazon web services (AWS)
  - AWS Policy Generator 
  - AWS IAM
- JSON

## Select Policy Type:
Begin by choosing the type of policy to suit your requirements. For this project, we will choose an IAM Policy. 

![---](https://imgur.com/LZkWbwr.jpg) 

We will use a Bucket from the Amazon AWS S3 console. For this project I will use a test bucket titled 'testmybuckets300963723832'. Click on the bucket's name to open it.

![---](https://imgur.com/aV6oqhL.jpg) 

Select the Properties tab within the bucket and copy the Amazon Resource Name (ARN).

![---](https://imgur.com/BICdvOn.jpg) 

![---](https://imgur.com/lmSrMqA.jpg) 

## Select AWS Service:
Navigate back to the AWS Policy Generator tool. Select ALLOW for the policy Effect. Note: AWS automatically defaults all policies Effect to DENY unless changed. 

For this project, we'll use Amazon S3 as our AWS Service and select the following Actions: GetObject, ListBucket, and PutObject. After your selections, the Actions should read '3 Action(s) Selected'. 

Then paste the copied ARN into the AWS Policy Generator's ARN field.

![---](https://imgur.com/IrvBHdc.jpg) 

## Actions Summary: 
Clicking on Add Statement will provide a summary of the policy generation steps taken so far.

![---](https://imgur.com/NKDBdg5.jpg) 

## Generate Policy
We will then click Generate Policy and a policy JSON document will be generated with our newly developed policy. 

![---](https://imgur.com/0hugpzK.jpg) 

We will copy the JSON policy generated for us.  

![---](https://imgur.com/951tCRE.jpg)  

## Create IAM Policy
Then in Amazon’s IAM console we will go to the Policy menu and select Create Policy.

![---](https://imgur.com/dd22GBF.jpg) 

Select the JSON options and paste our policy from the AWS Policy Generator. Select Review and Create to move to the next step.
![---](https://imgur.com/Q25NgY5.jpg)  

![---](https://imgur.com/cODZ5tR.jpg) 

Create a name of the new policy. I will name mine Tests3. Then click on Create Policy

![---](https://imgur.com/Em9pJsA.jpg) 

![---](https://imgur.com/7KBMfly.jpg) 

Our new policy was successfully created. A search for the policy was located, confirming it's creation.

![---](https://imgur.com/UahQ65l.jpg) 

![---](https://imgur.com/2c305zT.jpg) 

## Conclusion
In this project, we successfully created and implemented an AWS policy for S3, demonstrating a secure and efficient way to manage access for AWS resources.

## fin
