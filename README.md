# ansible-dynamic-hosts
ansible-dynamic-hosts
1.install ansible:amazon-linux-extras install ansible2
ansible --version-->see python version
2. install pip:yum install python-pip
3. pip install boto3
4.install awscli
5.enable plugins in ansible.cfg and add aws_ec2 -->plugin and all plugins mentioned above enable_pligins line in ansible.cfg file
6.create ansible dynamic inventory file:aws_ec2.yaml
7.ansible-inventory -i aws_ec2.yaml --list : gives all dynamic hosts list
8. ansible-playbook -i aws_ec2.yaml ping-playbook.yaml : runs ping playbook on dynamic hosts
