# x3ansible-digital-ocean

ansible-digital-ocean;
- web servers
- load balancer

```sh
ansible webservers --key-file ~/.ssh/id_ansible -i inventory -m ping
```

Update APT on all servers
```sh
ansible-playbook --key-file ~/.ssh/id_ansible -i inventory ansible-playbooks/apt.yml
```

Install Nginx
```sh
ansible-playbook --key-file ~/.ssh/id_ansible -i inventory ansible-playbooks/nginx.yml
```

Install php
```sh
ansible-playbook --key-file ~/.ssh/id_ansible -i inventory ansible-playbooks/php.yml
```

Deploy index.html
```sh
ansible-playbook --key-file ~/.ssh/id_ansible -i inventory ansible-playbooks/deploy_index.yml
```
