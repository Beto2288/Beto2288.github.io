---
layout: post
title: Quick Start with Boto3 and AWS
---


In this post, we’ll take a look at some basics examples of using Python scripts to interact with the infrastructure provided by Amazon Web Services (AWS).

Take in count if you want to replicate this with your own AWS account, you will need:
* An AWS account with admin or power user privileges.
* Internet connection and Linux shell environment.
* Some experience with Python and Bash command line interface.
* An EC2 instance with Python, Boto3 and AWS CLI tool configured. You can use the Amazon Linux AMI which has all these packets.

After you setup your environment you can check is all is configured running the following command:

![_config.yml]({{ site.baseurl }}/images/EC2_first_picture.png)

`Where the yellow part is the instance ID of your EC2 instance.`

## Examples of how to use some basics scripts:

**List Instances:**

![_config.yml]({{ site.baseurl }}/images/List_instances_1_1.png)

Results:

![_config.yml]({{ site.baseurl }}/images/List_instaces_2.png)

**Create an Instance:**

![_config.yml]({{ site.baseurl }}/images/Create_instance_1_1.png)

Results:

![_config.yml]({{ site.baseurl }}/images/Create_instance_2.png)

![_config.yml]({{ site.baseurl }}/images/Create_instance_3.png)

**Terminate an Instance:**

![_config.yml]({{ site.baseurl }}/images/Terminated_instances_1.png)

In this case the ID is our input for the `terminate_instance.py` script.

![_config.yml]({{ site.baseurl }}/images/Terminated_instances_2.png)

Results:

![_config.yml]({{ site.baseurl }}/images/Terminated_instances_3.png)

**Checking status of the instances:**

![_config.yml]({{ site.baseurl }}/images/Checking_status_instances_1.png)

Results:

![_config.yml]({{ site.baseurl }}/images/Checking_status_instances_2.png)

**Create a Bucket**

![_config.yml]({{ site.baseurl }}/images/Create_bucket1.png)

For this case we need to define the name of the bucket due to the restrictions and limitations of S3 (*Bucket names must be globally unique and, Bucket names must follow DNS naming conventions*).

![_config.yml]({{ site.baseurl }}/images/Create_bucket2.png)

![_config.yml]({{ site.baseurl }}/images/Create_bucket3.png)


There are a lot of ways to create different scripts, and every person will create and adapt the scripts based on their necessity. As last example here is one that I’ve made just playing with this:

![_config.yml]({{ site.baseurl }}/images/Combine_script1.png)

This script will create an instance and wait until change the state to running, then create one file with the details of the instance and also it’s uploaded to our S3 bucket.

![_config.yml]({{ site.baseurl }}/images/Combine_script2.png)

![_config.yml]({{ site.baseurl }}/images/Combine_script3.png)

![_config.yml]({{ site.baseurl }}/images/Combine_script4.png)

