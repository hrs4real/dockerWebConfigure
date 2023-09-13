# Ansible Playbook for Docker Configuration

Welcome to the Ansible playbook for configuring Docker effortlessly and setting up a web server using Ansible automation. This playbook allows you to perform the following tasks:

- Configure Docker effortlessly.
- Start and enable Docker services.
- Pull the latest httpd server image from the Docker Hub with ease.
- Run the Docker container smoothly and expose it to the public.
- Copy your HTML code to the /var/www/html directory and kickstart your web server in a blink.

Let's break down the setup into steps:

## Step 1: Installing Ansible
```shell
$ sudo yum install ansible -y
```
## Step 2: Create an Ansible Directory and Navigate into 'ansible'
```shell
$ mkdir ansible
$ cd ansible
```
## Step 3: Configuration with ansible.cfg
```shell
$ vim ansible.cfg
```
Add the following content to the ansible.cfg file:
```ini
[defaults]
remote_user = your_username
```
## Step 4: Create an Inventory File
Create an inventory file (e.g., inventory.txt) and add the IP address of your slave node.
## Step 5: Establish Password Access
Establish password access from the slave node to the master node.
## Step 6: Verify Connectivity
```shell
$ ansible all -m ping
```
## Step 7: Craft the docker.yml Playbook
Create a YAML file (e.g., docker.yml) and insert your Docker playbook code. You can find an example YAML code on my GitHub profile.
## Step 8: Validate Your Playbook
```shell
$ ansible-playbook docker.yml
```
## Step 9: Run Your Playbook
Your playbook should run successfully. Check the IP of your slave node and any other desired outcomes.

For detailed instructions and example YAML code, please refer to the docker.yml file in this repository.


# You can also check my blog on medium for a detailed explanation of docker.yml
https://medium.com/@hrs4real/simplifying-web-server-deployment-with-ansible-a-technical-guide-abdc748ad3e9

