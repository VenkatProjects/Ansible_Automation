# Ansible
## Automation_Ansible_Playbook

We have written Ansible YAML file to create an EC2 instance

![ec2_create](https://user-images.githubusercontent.com/67817741/181302307-394c896c-a7b4-4644-9f9a-c6a5b4b8ae20.PNG)

Before Running the YAML file, need to be check syntax

   ansible-playbook ec2_instance.yml --syntax-check

![syntax](https://user-images.githubusercontent.com/67817741/181302390-18d0f739-5605-4ab0-b550-8bb3b54b3163.PNG)

if you are not getting any error, we are good to run the ansible-playbook

After running, We are getting below error. It says, boto needs to be installed.

![boto_error](https://user-images.githubusercontent.com/67817741/181307737-a74b47a9-b492-47f2-b0ea-8f23000cb81e.PNG)

So we need to run the below command to install boto

   ### sudo yum install -y python-pip

once installed pip,then run the below command to install boto & boto 3 version

  ### sudo pip install boto boto3

after everything installed, again we're facing issue. It says #### "Handlers were checked" which means

![handler](https://user-images.githubusercontent.com/67817741/181317678-1675508b-a14b-48fe-ad75-f7b7a3bb46a2.JPG)


we need to provide Credentials details. Either you can add into YAML file or run like below

### export AWS_ACCESS_KEY="aws access key generated from AWS"

### export AWS_SECRET_ACCESS_KEY=" aws secret key generated from AWS"

once everything added, run the below command 

	ansible-playbook ec2_instance.yml

Now we have successfully launched 

![created_ec2](https://user-images.githubusercontent.com/67817741/181318233-26da700b-01bc-473f-8bba-82466ee0f2dc.JPG)

### Before Run Ansible script

![before](https://user-images.githubusercontent.com/67817741/181318478-a3520838-5a7b-4e79-bf1b-3eccafbe006e.JPG)

### After Run Ansible Script

![after](https://user-images.githubusercontent.com/67817741/181320716-55b90c9e-d429-4793-a075-38844b86c1e4.JPG)

