### Setup dengan ansible

## Install Ansible

Panduanya ada disini
https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

## Config server
Edit file hosts, sesuaikan dengan host/ip server yang akan disetup ssh_key sesuaikan dg private key untuk masuk ke server

## Create User Admin
```ansible-playbook -i hosts user.yml```

## Install Nginx
```ansible-playbook -i hosts install_nginx.yml```

## Install PHP 7.4
```ansible-playbook -i install_php7.4.yml```

## Install Docker dan Docker Compose
```ansible-playbook -i install_docker.yml```

## Install Maria DB redis
Sesuaikan file docker-compose.yml dengan keinginan anda seperti port yng berjalan, password dll
```ansible-playbook -i install_mariadb_redis.yml```

## Setup UFW
```ansible-playbook -i setup_ufw.yml```

## Install Composer
```ansible-playbook -i install_composer.yml```

## Setup config nginx vhost
ubah vars di file config_nginx.yml dengan domain anda lalu jalankan
```ansible-playbook -i install_composer.yml```

## Install Cerbot
ubah vars domain dengan domain anda lalu jalankan
```ansible-playbook -i install_composer.yml```

Selesai upload ke document root /home/admin/namadomainanda/public/