## Ansible Script to Terminate EC2 Instance

Wrritten a YAML file to Terminate EC2 Instance

### Terminate YAML File

![terminate_file](https://user-images.githubusercontent.com/67817741/181593462-dab91fda-f8a8-402b-809c-1eb4c894066e.JPG)

### EC Instance Running Window

![instance](https://user-images.githubusercontent.com/67817741/181593759-26fab2cf-a981-4520-b6f0-0957d864d5ff.JPG)

Note: Higlighted instance id will be terminiated

### Ansible Command

After checking the syntax, Run below command

	ansible-playbook terminate.yml
		
![terminiating](https://user-images.githubusercontent.com/67817741/181594061-6d2df519-7345-4bcc-99ce-5f57df28be76.JPG)

### Final Output in AWS Console.

![Terminiated](https://user-images.githubusercontent.com/67817741/181594293-ecdc0428-3522-4749-80c3-9704cdafcdb2.JPG)

We have successfully terminated the insatce using ansible automation tool.