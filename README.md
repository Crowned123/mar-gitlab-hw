# Домашнее задание к занятию «Система мониторинга Zabbix»
# Задание 1
![image](https://github.com/user-attachments/assets/1977325c-43be-4178-9efe-9b513da4a90f)
- wget https://repo.zabbix.com/zabbix/6.4/ubuntu-arm64/pool/main/z/zabbix-release/zabbix-release_6.4-1+ubuntu22.04_all.deb
- dpkg -i zabbix-release_6.4-1+ubuntu22.04_all.deb
- apt update
- apt install zabbix-server-pgsql zabbix-frontend-php php8.1-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent
- sudo -u postgres createuser --pwprompt zabbix
- sudo -u postgres createdb -O zabbix zabbix
- zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix
- nano /etc/zabbix/zabbix_server.conf
- DBPassword=password
- systemctl restart zabbix-server zabbix-agent apache2
- systemctl enable zabbix-server zabbix-agent apache2
- git commit -m "Z1"
- git push origin  

# Задание 2








