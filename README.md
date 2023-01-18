# Домашнее задание к занятию 9.2 "Zabbix. Часть 1`" - `Рыженко Назарий`

### Задание 1 

Установите Zabbix Server с веб-интерфейсом.
![image](https://user-images.githubusercontent.com/106932460/213180154-32227686-49ef-451a-9aa8-4a96d5073960.png)
![image](https://user-images.githubusercontent.com/106932460/213161694-cd1ab9ef-5123-45eb-b21f-994b06eeb0cb.png)
Так как Zabbix поддерижвает pgsql от 13, то устанавливал его из репозитория https://www.postgresql.org/media/keys/ACCC4CF8.asc

---

### Задание 2 

Установите Zabbix Agent на два хоста.
```bash
# wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-4%2Bdebian10_all.deb
# dpkg -i zabbix-release_6.0-4+debian10_all.deb
# apt update
# apt install zabbix-agent
# systemctl restart zabbix-agent
# systemctl enable zabbix-agent
```
*Приложите скриншот раздела Configuration > Hosts, где видно, что агенты подключены к серверу.*
*Приложите скриншот лога zabbix agent, где видно, что он работает с сервером.*
*Приложите скриншот раздела Monitoring > Latest data для обоих хостов, где видны поступающие от агентов данные.*
*Приложите текст использованных команд в GitHub.*

---
## Задание со звёздочкой*

Это дополнительное задание. Его выполнять не обязательно. На зачёт это не повлияет. Вы можете его выполнить, если хотите глубже разобраться в материале.

### Задание 3* 

Установите Zabbix Agent на Windows (компьютер) и подключите его к серверу Zabbix.

*Приложите скриншот раздела Latest Data, где видно свободное место на диске C:*
