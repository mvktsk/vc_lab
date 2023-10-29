1. Create virtual machine in the yandex cloud
Платформа Intel Ice Lake
Гарантированная доля vCPU 100%
vCPU 2
RAM 4 ГБ
Объём дискового пространства 500 ГБ

2. Install docker https://docs.docker.com/engine/install/ubuntu/

3. Install nginx https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-20-04
4. Copy ./init-db folder and ./docker-compose.yml to ~/projects/virto_lab
5. Run docker-compose
6. Change admin password
7. Copy ./admin.ecom-lab-nsu.ru.conf and ./store.ecom-lab-nsu.ru.conf to /etc/nginx/sites-available
8. Create simlink for ./admin.ecom-lab-nsu.ru.conf and ./store.ecom-lab-nsu.ru.conf to /etc/nginx/sites-enabled

`sudo ln -s /etc/nginx/sites-available/admin.ecom-lab-nsu.ru.conf /etc/nginx/sites-enabled/admin.ecom-lab-nsu.ru.conf`

`sudo ln -s /etc/nginx/sites-available/store.ecom-lab-nsu.ru.conf /etc/nginx/sites-enabled/store.ecom-lab-nsu.ru.conf`
