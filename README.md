# ansible_wordpress-site
wordpress,apache,php,mysql configuration to lunch wordpress site

**roles-**

 +-- roles
     +-- main
         +--tasks/main.yml
     +--php
        +--tasks/main.yml
     +--mysql
        +--defaults/main.yml
        +--tasks/main.yml
     +--wordpress
        +--tasks/main.yml
        +--handlers/main.yml
        

- create hosts file in your current directory:-

- encrypt mysql password, database, user password using ansible-vault

- run this palybook with command:-
- 
 **ansible-playbook -i hosts wordpress/playbook.yml -s --vault-password-file vault_pass**
(my vault password stored in "vault_pass" file)

 or
 
 **ansible-playbook -i hosts wordpress/playbook.yml -s --ask-vault-pass**
