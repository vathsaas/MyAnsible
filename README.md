# SREChallenge
The above script is  for automating a standalone EC2 Instance on AWS and configuring it to serve a basic HTML page.

Requirements:-
Ansible 2.0 or greater
Python 2.7 or greater
Pip
boto3
AWS-CLI

Details related to the scripts:-

1> There are 3 files in the repository namely main.yml, Instance_setup.yml, Instance_config.yml
2> main.yml file is for orchestrating the entire setup which has references to both Instance_setup.yml and Instance_config.yml
3> Instnace_setup.yml is a ansible script to setup a EC2 instance on AWS with additonal thing like securing the instance that will be created.
4> Instance_config.yml is a ansible script to configure the instance by setting up nginx (webserver), Self signed SSL certificate, setting up a basic html page and running tests t check the configurations.



Steps to Execute the script:-

1> From any path on your system clone the repository
   git clone https://github.com/vathsaas/SREChallenge.git
2> Open the SREChallenge folder 
3> Open Instance_setup.yml and make changes on lines
4> After the changes are done we are ready to execute the script
5> Execute the folowing command to  trigger the execution
   ansible-playbook main.yml
   
