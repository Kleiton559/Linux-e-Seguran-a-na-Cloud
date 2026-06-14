# Publicação WordPress
## Nível escolhido
Nível 3 - Avançado
## Rota escolhida
Nginx
## Componentes usados
- Servidor web: nginx
- PHP:php v8.5.4 
- Base de dados: mariaDB 11.8.6
- WordPress:
## Pasta de publicação
## URL de acesso
link de acesso ao Wordpress - http://192.168.1.135/wp-admin/setup-config.php 
## Comandos principais utilizados
sudo apt update && sudo apt upgrade -y

sudo apt install nginx -y
sudo systemctl enable nginx
sudo systemctl start nginx

systemctl status nginx

sudo apt install php-fpm php-mysql php-cli php-curl php-gd php-xml php-mbstring php-zip unzip -y
php -v

sudo apt install mariadb-server mariadb-client -y
sudo systemctl enable mariadb
sudo systemctl start mariadb

cd /tmp
wget https://wordpress.org/latest.tar.gz
tar -xvzf latest.tar.gz

sudo mv wordpress /var/www/html/
sudo chown -R www-data:www-data /var/www/html/wordpress
sudo chmod -R 755 /var/www/html/wordpress

## Resultado obtido
Consegui instalar o Wordpress, Segue abaixo a evidencia da pagina inicial do meu Wordpress instalado


## Limitações encontradas
