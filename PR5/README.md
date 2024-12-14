# **СДССиЛ Практическая работа номер 5 - Threat Hunting**
**Выполнил - Панков Евгений Ромуальдович**
# **Перейдем к процессу выполнения работы:**
## **1. Результат развертывания ВМ для выполнения работы:**
### **1.1 ВМ - Сервер (`Ubuntu`):**
![image](Screenshots/1.png)
### **1.2 ВМ - Клиент (`Ubuntu`):**
![image](Screenshots/2.png)
### **1.3 ВМ - Атакующая (`Kali`):**
![image](Screenshots/3.png)
### **1.4 Проверка связи между ВМ:**
![image](Screenshots/4.png)
## **2. Установка на серверную ВМ Сервера `Wazuh`:**
![image](Screenshots/5.png)
### **2.1 Проверка WEB-интерфейса `Wazuh-сервера`:**
![image](Screenshots/6.png)
## **3. Установка агента на клиентскую ВМ:**
![image](Screenshots/7.png)
![image](Screenshots/8.png)
### **3.1 Проверка отображения подключенного агента на `Wazuh-сервере`:**
![image](Screenshots/9.png)
## **4. Установка `Suricata IDS` на клиентскую ВМ:**
![image](Screenshots/10.png)
### **4.1 Установка набора правил для `Suricata`:**
![image](Screenshots/11.png)
### **4.2 Настройка конфигурации `Suricata IDS`:**
![image](Screenshots/12.png)
![image](Screenshots/13.png)
![image](Screenshots/14.png)
### **4.3 Настройка сбора логов и передачи в `Wazuh-сервер`:**
![image](Screenshots/15.png)
### **4.4 Проверка логов `Suricata` на `Wazuh-сервере`:**
![image](Screenshots/16.png)
![image](Screenshots/17.png)
## **5 Осуществление проверки работы правил `Suricata`:**
### **5.1 На ВМ Атакующая-Kali выполним ping на Клиентскую ВМ:**
![image](Screenshots/18.png)
### **5.2 Проверка на `Wazuh-сервере` наличия обнаружения активности и предупреждений:**
![image](Screenshots/19.png)
![image](Screenshots/20.png)
## **6 Установка `YARA` на клиентскую ВМ:**
### **6.1 Выполнение команд для установки `YARA` на Клиентсую ВМ:**
![image](Screenshots/21.png)
### **6.2 Проверка установки:**
![image](Screenshots/22.png)
###  **6.3 Исправление ошибки:**
![image](Screenshots/23.png)
### **6.4 Установка набора правил для `YARA`:**
Ошибки из-за отсутствия VPN

![image](Screenshots/24.png)
### **6.5 Создание скрипта `yara.sh` для получения данных сканирования в `Wazuh-сервер`:**
![image](Screenshots/25.png)
### **6.6 Выдача прав на скрипт `yara.sh`:**
![image](Screenshots/26.png)
### **6.7 Настройка сбора логов и передачи в `Wazuh-сервер`:**
![image](Screenshots/27.png)
## **7 Настройка Серверной ВМ для работы с `YARA`:**
![image](Screenshots/28.png)
![image](Screenshots/29.png)
![image](Screenshots/30.png)
## **8. Проверка результата подключения `YARA` к `Wazuh-серверу`:**
### **8.1 Создание скрипта для проверки `YARA` на Клиентской ВМ:**
![image](Screenshots/31.png)
![image](Screenshots/32.png)
### **8.2 Отображение результата в `Wazuh-сервере`:**
![image](Screenshots/33.png)
