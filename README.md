1. Create redhat 8 ec2 instance

2. switch user to  root

3. install commands
   - cmd : yum update

4. check python is installed or not by following command
      cmd : python --version
      if not then install python2 or python3
      - if you want to install python2 then hit following cmnds
         - cmd : yum install python2
      -if you want to install python3 then hit following cmnds
         - cmd : yum install python3

5. check pip is installed or not by following command
      cmd : pip --version
      if not then install pip2 or pip3
      - if you want to install pip2 then hit following cmnds
         - cmd : dnf install python2-pip
      -if you want to install pip3 then hit following cmnds
         - cmd : dnf install python3-pip

6. Install ansible by using pip
      - if you have installed python2 run following cmd
         cmd : pip2 install ansible
      - if you have installed python3 run following cmd
         cmd : pip3 install ansible

7. change ansible_python_interpreter = python2 for python2
   else  ansible_python_interpreter = python2  for python3 in e2eproject/inventory file 

8. change credentials for creating aws ec2 instance in roles/tomcat_aws/default/main.yml file

9. change appropriate java jdk version in roles/tomcat/tasks/install_packages.yml file

10. run cmd : ansible-playbook deploy.yml file

11. done 
      

        
      
