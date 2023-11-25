# Ansible Refactoring & Static Assignments (Imports and Roles)

## STEP 1.  **Jenkins job enhancement**

1. Still maintaining my infrastructure from the last project, on my `Jenkins-Ansible` server, i created a directory called `ansible-config-artifact` and mdoified its permissions by running the following code;

```bash
# Create the directory
sudo mkdir /home/ubuntu/ansible-config-artifact

# Modify its permissions
sudo chmod -R 0777 /home/ubuntu/ansible-config-artifact
```

2. I installed ansible on the server and checked the version of ansible installed by running the following lines of code;

 ```bash 
sudo apt update
sudo apt install ansible -y

# Check version of Ansible
ansible --version
```

![Screenshot](https://github.com/ardamz/my-demo/blob/main/project12/Mkdir.png)


3. On my Jenkins web cosole, I installed the `Copy Artifact` plugin.

4. I created a new project called `save_artifacts`, and this project will be triggered by the completion of my exisiting `ansible` project.
