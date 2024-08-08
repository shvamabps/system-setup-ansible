# Requirements in Ubuntu 
1. Python3-pip
2. Ansible

# Installation
1. Python3-pip:
```bash
sudo apt-get install python3-pip -y
```
2. Ansible
```bash
python3 -m pip install ansible 
```

# Update `hosts.ini` file
1. Fill out the details in the `hosts.ini` file based on the below code snippet

```ini
[ubuntu_servers] # group name
<hosts> ansible_user=<username> ansible_become=true ansible_ssh_pass=<ssh password> ansible_become_password=<root password>
```

# Execution
1. Change the permission of `setup.sh` file
```bash
chmod +x ./setup.sh
```
2. Execute the file
```bash
./setup.sh
```
