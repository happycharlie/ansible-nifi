# ansible-nifi
ansible project for installing nifi/nifi registry

Server info (virtualbox)
Centos-POC-01 : 192.168.99.102
Centos-POC-02 : 192.168.99.103

setup keyless login
   ssh-copy-id xxxx@192.168.99.102
   ssh-copy-id xxxx@192.168.99.103

setup no passwd for sudoers
   visudo
      comment out %wheel ALL=(ALL)     ALL
      uncomment %wheel ALL=(ALL)     NOPASSWD: ALL

test the setup 
   ansible all -i ./hosts -m ping

