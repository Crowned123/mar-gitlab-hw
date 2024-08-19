# Домашнее задание "Система мониторинга Zabbix. Часть 2"
# Задание 1 
![image](https://github.com/user-attachments/assets/eaa637a3-71d7-4f31-b8da-e00af68904e8)
- CPU system.cpu.util[,user]
- RAM vm.memory.size[pused]
# Задание 2 и # Задание 3 
![image](https://github.com/user-attachments/assets/c2266614-3a9f-499f-b1b8-852c19b6d718)
![image](https://github.com/user-attachments/assets/5d127028-556b-476b-a504-2c58c3546002)
![image](https://github.com/user-attachments/assets/7fdfdcdc-a0a8-45cc-8ba5-a959dbc2031a)

# Задание 4 
![image](https://github.com/user-attachments/assets/e3a57b46-8d6a-4937-b467-8993ba836851)

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
![image](https://github.com/user-attachments/assets/3357cfcc-6901-4554-ab6f-83cbbbeaf843)
![image](https://github.com/user-attachments/assets/46bd895f-a44f-45c4-b461-44956e101cfc)
![image](https://github.com/user-attachments/assets/2c0670f0-67eb-432f-849c-d3aa476ff6e2)
![image](https://github.com/user-attachments/assets/d2835b6f-5201-4d64-b49e-1a452a1d7012)
- git commit -m "Z2"
- git push origin










