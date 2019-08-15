# ansible-wordpress
Ansilbe Roles for Setup Wordpress
- Buatlah user biasa di Server dan jadikan Sudo.
- Setup SSH-Key Pair dari Ansible Host ke Server. Ref: https://www.lukmanlab.com/cara-login-ssh-server-tanpa-password/
- Untuk menjalankan Ansible Roles ini ada beberapa file yang perlu diedit seperti file hosts dan file variable didalam roles.

## File Hosts
- Sesuaikan IP Address server
- Sesuaikan User 
- [all:vars] sesuaikan password user tsb.

## Sesuaikan Variable di Nginx Roles (Roles - 3nginx)
- Di roles - 3nginx - vars - main.yml ~ Silahkan sesuaikan domain yang akan digunakan

## Menjalankan Ansible (didalam folder ansible-wordpress)

`$ ansible-playbook -i hosts main.yml`