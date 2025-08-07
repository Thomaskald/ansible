# Deploy the app to a Vagrant VM
While being in the directory that each Vagrant VM exists, you run the following command in terminal to start each VM:
vagrant up
Move to the directory that has the ansible.cfg and hosts.yaml and run the playbooks
For Frontend-Backend
ansible-playbook -i hosts.yaml playbooks/app.yaml
For Database 
ansible-playbook -i hosts.yaml playbooks/postgres.yaml
You can use the app from the http://192.168.56.11

# Run the app with Docker 
While being in the directory that Vagrant VM exists, you run the following command in terminal to start the VM:
vagrant up 
Move to the directory that has the ansible.cfg and hosts.yaml and run the playbooks
ansible-playbook -i hosts.yaml playbooks/docker.yaml
ansible-playbook -i hosts.yaml playbooks/docker-deploy.yaml 
You can use the app from the http://192.168.56.12
