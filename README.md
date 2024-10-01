Очереди RabbitMQ - AAleksandr Mihajlov SYS34  
  
**Задание 1. Установка RabbitMQ**  
  
Используя Vagrant или VirtualBox, создайте виртуальную машину и установите RabbitMQ. Добавьте management plug-in и зайдите в веб-интерфейс.  
Итогом выполнения домашнего задания будет приложенный скриншот веб-интерфейса RabbitMQ.  
  

![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/1a.png)  
  
**Задание 2. Отправка и получение сообщений**  
  
Используя приложенные скрипты, проведите тестовую отправку и получение сообщения. Для отправки сообщений необходимо запустить скрипт producer.py.  
Для работы скриптов вам необходимо установить Python версии 3 и библиотеку Pika. Также в скриптах нужно указать IP-адрес машины, на которой запущен RabbitMQ, заменив localhost на нужный IP.  
Зайдите в веб-интерфейс, найдите очередь под названием hello и сделайте скриншот. После чего запустите второй скрипт consumer.py и сделайте скриншот результата выполнения скрипта  
В качестве решения домашнего задания приложите оба скриншота, сделанных на этапе выполнения.  
  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/2a.png)  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/2b.png)  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/2c.png)  
  
**Задание 3. Подготовка HA кластера**  
  
Используя Vagrant или VirtualBox, создайте вторую виртуальную машину и установите RabbitMQ. Добавьте в файл hosts название и IP-адрес каждой машины, чтобы машины могли видеть друг друга по имени.  
осле этого ваши машины могут пинговаться по имени.
Затем объедините две машины в кластер и создайте политику ha-all на все очереди.
В качестве решения домашнего задания приложите скриншоты из веб-интерфейса с информацией о доступных нодах в кластере и включённой политикой.
Также приложите вывод команды с двух нод.  
  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/3.png)  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/3.1.png)  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/3.2.png)  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/3.3.png)  
![alt text](https://github.com/AleksandrMihajlov/SDB-11-04/blob/main/3.4.png)  
  
*C rabbitmqadmin get queue='hello' возникли проблемы, скриншот 3.4*  
*Видимо где-то допустил ошибку с добавлением "админа"*