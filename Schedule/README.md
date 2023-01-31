In this example, the EC2 instance is stopped and started using the ec2 module. The instance ID is passed as a variable to the playbook, and can be defined in a separate file or passed in as an extra variable on the command line.

The when argument is used to check the current hour in the ansible_date_time fact, and only perform the stopping or starting of the instance if the hour matches the desired time.

The playbook is then scheduled to run at 11 PM and 10 AM IST using the cron module. The minute argument is set to 0 to run the playbook on the hour. The hour argument is set to 22,10 to run the playbook at 11 PM and 10 AM IST, respectively. The job argument specifies the command to run the playbook.

This is just a basic example and can be customized to fit your specific use case. You can find more information on using the EC2 and cron modules in the Ansible documentation.
