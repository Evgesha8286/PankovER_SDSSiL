# **СДССиЛ Практическая работа номер 1 - Аггрегация и сбор логов**

Выполнил - Панков Евгений Ромуальдович

## **1. Создаем 2 виртуальные машины на базе ОС Debian 12 и обеспечиваем между ними сетевой обмен (Использовался VirtualBox как клиент виртуализации):**

   ![image](Pictures/1.png)

   ![image](Pictures/2.png)

   ![image](Pictures/3.png)

## **2. Включаем на 1-ой (сервере) из ВМ передачу логов по протоколу rsyslog на 2-ую ВМ (клиент):**

### ***2.1 Устанавливаем и настраиваем rsyslog на сервере и клиенте:***

![image](Pictures/4.png)

### ***2.2 Проверяем работоспособность rsyslog на сервере и клиенте:***

![image](Pictures/5.png)

### ***2.3 Включаем UDP и TCP соединение:***

![image](Pictures/6.png)

### ***2.4 Устанавливаем правила на сервере:***

![image](Pictures/7.png)

### ***2.5 Установливаем правила на клиенте:***

![image](Pictures/8.png)

### ***2.6 Проверяем получения логов на сервере:***

![image](Pictures/9.png)

![image](Pictures/10.png)

## **3. Устанавливаем и настраиваем получение логов на сервере с использованием Loki:**

### ***3.1 Устанавливаем и редактируем compose-файл на сервере:***

![image](Pictures/11.png)
![image](Pictures/12.png)

### ***3.2 Запускаем Loki:***

![image](Pictures/13.png)

### ***3.3 Редактируем promtail на клиенте:***

![image](Pictures/14.png)

### ***3.4 Редактируем compose-файл для promtail:***

![image](Pictures/15.png)

### ***3.5 Запускаем promtail на клиенте:***

![image](Pictures/16.png)

### ***3.6 Просматриваем логи клиента в Grafana Loki:***

![image](Pictures/17.png)

![image](Pictures/18.png)


## **4. Устанавливаем и настроиваем получение логов на сервере с использованием Signoz**

Установка Signoz согласно инструкции - <https://signoz.io/docs/install/docker/#install-signoz-using-docker-compose>

Установка приложения sample-nodejs-app согласно инструкции - <https://github.com/SigNoz/sample-nodejs-app/>

### ***4.1 Запускаем Signoz:***

![image](Pictures/19.png)
   
![image](Pictures/20.png)
   
![image](Pictures/21.png)

### ***4.2 Редактируем конфигурации на клиенте для отправки данных в Signoz:***

 ![image](Pictures/22.png)

### ***4.3 Запускаем клиентское приложение:***

 ![image](Pictures/23.png)

### ***4.4 Проверяем получение логов в Signoz:***

 ![image](Pictures/24.png) 
 
 ![image](Pictures/25.png)
