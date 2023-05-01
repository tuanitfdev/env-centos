mv /etc/ansible/ansible.cfg  /etc/ansible/ansible.cfg.bak
cp ansible.cfg /etc/ansible/
ansible-galaxy install -r requirements.yml
ansible-playbook site.yml -i inventory.txt
