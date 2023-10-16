# Hands on With Terraform And Cloud

What is Terraform?  
Terraform is an infrastructure as Code(IaC) tool that lets you build, change, and version both cloud and on-premises resources.(Automated).  

Terraform is:  
1) Cloud Agnostic: Works with popular Cloud Provider like AWS, Azure, Cloud and Oracle.  

2) It uses Declarative language: (HCL (HashiCorp Configuration Language)).  

3) "Agentless" and "Masterless": Doesn't require any agent or any server, meaning it runs independently.  

Terraform: Use Cases  

1) Resource Provisioning on Cloud Providers.  
    "Plugins" connected to "Providers".  
    MultiCloud deployments.  

2) Resource Provisioning on "vmware" environments. 
    Can work in multicloud environmnets and Private cloud or Premise environments.  

3) Combine with multiple tools together:  
    Ansible  
    Kubernetes  

# How Terraform helps?  
Terraform is one of the main tools in the DevOps Universe.  

Terraform is part of the scope of the Professional who works with cloud.  

Terraform is widely used by large companies to provision their infrastructure.  

Terraform is the Evolution of the manual tasks. It is going to replace manual task when it comes to provision workloads and working with automation in the cloud workspace.  

# How does Terraform Work?  

Terraform has configuration files.  

main.tf  
resources.tf  
variables.tf  

The tf extension is for Terraform files. *.tf  

These are configuration files that have description we want terrafomr to execute while provisioning.  

Terraform which is a tool, that is a binary that can be installed in our machine regardless of operating system(Linux, Windows, Mac).  

Terraform looks for these files and provision what we want to do with our resources.  

Terraform provision the resources and keeps record in state files. Next time we run, it checks the state and provision the new changes.  

# Hands-on With Terraform And AWS  

Using terraform to provision resource in AWS.  

Use VS code to create configuration files.  
Terraform is going to look for this files and use that to provision resources.  

Amazon Simple Storage Service(Amazon S3): S3 is just a starter service in AWS where we can create a bucket. Bucket is like a dropbox that you can store files in AWS in a very safe way.   

you can do it manually.  
Create a S3 Service.  

Create a Free AWS Account. Sign up for free. The code might takes around five minutes to arrive.  

Go to AWS Console. Type S3 in the Search bar. Create a new bucket using UI. And you can create a bucket step by step.  

But Creating bucket can be done using terraform configuration file.  

Using VS to do this.  
*** Install the terraform Extension in Visual Studio.**   
Create a new folder to keep things organize.  

In this case,  
I have created a folder called cloudwarmup  
and inside I have created a folder called live2-terraform-aws.    
Inside the folder I have terraform configuration file called main.tf.    

The first step we need to do is to specify the cloud provider.  
In this case it is AWS.  

Look in the terraform documentation.  

Go to https://registry.terraform.io/ and click in the browse and go to providers.  

Click on AWS and Go to Documentation.  

Look for the Example Usage and start writing the configuration file.  

-- Give the type of the providers and version.  
--Give the region  
-- Create a resource   
  aws_s3_bucket  
  s3_bucket  
  bucket_name *** bucket name should be unique.***   

Install the terraform in your local machine and connect the terraform with your aws account.    
In this project,    
Instead of installing the terraform in your local machine, use it from the AWS service that gives you shell in the browser and we can do things from there.  

Install terrafomr in your cloud shell.

go to documentation--> linux --> Amazon linux.

Follow the instructions to install the terraform from this link below:  
https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli

After this Step,
In Actions tab, Upload the main.tf file.
if ther are errors, 
rm main.tf file  
then run,  
$ terraform init 

$ terraform plan

$ terraform apply  

Now the bucket has been created.

Upload the image in the add files section and give the public access permission.

Write the public policy and update the restrictions.




































