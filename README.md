# sample_app


## Ansible automation deployment of a todo sample application

### What is this repository for? ###
#### with this repositiry you can easyly automate a deployment of an application to a preexisting virtual machine
#### there is no need for additional configuration or installing of any software, everithing will be confiigured and installed by the ansible playbook 

### Application architecture overview
![Scheme](images/app_overview.png)

### Ansible automation workflow overview
![Scheme](images/workflow.png)

### Control Node requirements
##### For your control node (the machine that runs Ansible), please refer to this hyperlynk: [Installing Ansible on specific operating systems](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-on-specific-operating-systems)

### Managed Nodes requirements
##### Although you do not need a daemon on your managed nodes, you do need a way for Ansible to communicate with them. For most managed nodes, Ansible makes a connection over SSH and transfers modules using SFTP. If SSH works but SFTP is not available on some of your managed nodes, you can switch to SCP in ansible.cfg. For any machine or device that can run Python, you also need Python 2 (version 2.6 or later) or Python 3 (version 3.5 or later).


### 

#### how to run ansible playbook deployment?

1. clone the repository `git clone repository_url`
2. after cloning the repository, update the __hosts.yaml__ file, hosts value with yout managed node public ip address. (if you prefer to access the application on a specific port you can update the application_port_mapping value to your desired needs, inside the __portvars.yaml_ file)
3. run the command  `ansible-playbook playbook.yaml`
4. waiti untill it finishes you should see the following output: 

<code>

<code>

