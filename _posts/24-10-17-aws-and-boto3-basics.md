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

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
