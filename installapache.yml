- hosts: all_host
  remote_user: ansadmin
  become: yes
  gather_facts: no
  pre_tasks:
   - name: 'install python'
     raw: 'sudo yum -y install python'
  tasks:
   - name: install httpd*
     yum: name=httpd state=latest
   - service:
       name: httpd
       state: started
       enabled: yes
