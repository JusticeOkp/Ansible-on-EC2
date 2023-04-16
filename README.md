# Ansible-on-EC2
Ansible Installation &amp; Configuration on AWS

## Steps
1. Create two EC2 instance: Launch the EC2 instances on AWS and ensure that it has the necessary permissions and security groups to interact with the host you want to configure. Make 1 the main and the other the sub-main.
2. Download putty and connect to the EC2 instances. Set up SSH access to the host you want to configure by generating an SSH key pair and adding the public key to the host's authorized_keys file.
3. Install Ansible on the EC2 instance by running the following command in the terminal: "sudo apt-get update", "sudo apt-get install ansible". Make sure you update the instances and also download python on the sub-main instances.
4. Create an inventory file: Create an inventory file on the EC2 instance that lists the hosts you want to configure.
5. Create a playbook that specifies the tasks you want to perform on the, mine was a simple playbook that installed the latest version of the apache2 package on all hosts in the inventory file.
6. Use the ansible-playbook command to run the playbook on the hosts listed in the inventory file. "ansible-playbook <play book name>"
