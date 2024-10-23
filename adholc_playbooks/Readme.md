Get the Facts of a Host 54.172.189.220
```
ansible ubuntu@54.172.189.220 -i inventory.ini -m setup
```

Ansible play book can be executed with the following command
```
ansible-playbook -i inventory.ini install_httpd.yaml
```

If there are 10 tasks and we need to install 8 tasks ans 2 can be skipped Ansible play book can be executed with the following command
```
ansible-playbook -i inventory.ini install_httpd.yaml --step
```

If we wanted to check what is going to chnage with the Ansible playbook execution 
```
ansible-playbook -i inventory.ini install_httpd.yaml --check
```

Run Ansible with verbosity mode
```
ansible-playbook -i inventory.ini install_httpd.yaml -V
ansible-playbook -i inventory.ini install_httpd.yaml -VV
ansible-playbook -i inventory.ini install_httpd.yaml -VVV
ansible-playbook -i inventory.ini install_httpd.yaml -VVVV
```