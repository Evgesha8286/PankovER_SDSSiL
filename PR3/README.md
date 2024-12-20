# **СДССиЛ Практическая работа номер 3 - WAZUH**
**Выполнил - Панков Евгений Ромуальдович**
# **Перейдем к процессу выполнения работы:**
## **Шаг 1 - Результат установки и настройки 2 ВМ (Сервер и Клиент):**
### **Проверим Ip адреса 2 ВМ:**
![image](Screenshots/1.png)
![image](Screenshots/2.png)

## **Шаг 2 - Проверка связи между двумя ВМ:**
### **Пропингуем две ВМ между собой:**
![image](Screenshots/3.png)

## **Шаг 3 - Установка Wazuh-сервера на серверной ВМ:**
![image](Screenshots/4.png)
### **Проверим результат установки и перейдем в web-интерфейс Wazuh:**
![image](Screenshots/5.png)
![image](Screenshots/6.png)

## **Шаг 4 -Перейдем к установке агента на клиентской ВМ:**
### **Сгенерируем команды в web-интерфейсе Wazuh:**
![image](Screenshots/7.png)
### **Выполним команды на клиентской ВМ:**
![image](Screenshots/8.png)
## **Шаг 5 - Проверка отображения нового агента в web-интерфейсе Wazuh**
![image](Screenshots/9.png)
### **Отбразим детектор уязвимостей для конкретного агента:**
![image](Screenshots/10.png)

## **Шаг 6 - Проверим активность проверки целостности файлов:**
![image](Screenshots/11.png)

## **Шаг 7 - Настроим выявление уязвимостей:**
![image](Screenshots/12.png)

## **Шаг 8 - Настроим выявление скрытых процессов:**
### **Установим нужные пакеты:**
![image](Screenshots/13.png)
### **Изменим значение нужного параметра:**
![image](Screenshots/14.png)

## **Шаг 9 - Настроим выявление SQL-иньекций:**
### **Установим нужные для работы пакеты:**
![image](Screenshots/15.png)
### **Изменим файл конфигурации:**
![image](Screenshots/16.png)

## **Шаг 10 - Настроим выявление web shell attack:**
### **Сразу перейдем к изменению файла конйигурации:**
![image](Screenshots/17.png)

## **Шаг 11 - Проверка обнаружения атаки:**
### **Wazuh определил SQL-иньекцию после осуществления таковой на клиентскую машину:**
![image](Screenshots/18.png)
![image](Screenshots/19.png)
