# startupvps
### install ansible
### edit hosts
```
edit /etc/ansible/hosts like this:
[vps]
xxx.xxx.xxx.xxx
as a group
```
### play the book
```
ansible-playbook ./start.yml -uroot -k
maybe you need intall sshpass for the parameter '-k'

ansible-playbook ./start.yml -uroot -b
install all tasks
or 
install one tasks:
ansible-playbook ./start.yml -t init -uroot -b
```
you can custom your own config files at some tasks's files dirctory.
