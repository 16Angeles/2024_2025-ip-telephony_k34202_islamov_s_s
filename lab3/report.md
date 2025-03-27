University: ITMO University

Faculty: PIn

Course: IP-telephony

Year: 2024/2025

Group: K34202

Author: Islamov Sergey Sergeevich

Lab: Lab3

Date of create: 25.03.2025

Date of finished: 

# Лабораторная работа №3 "Использование Asterisk в качестве SIP proxy"

## Цель работы

Изучить программный комплекс Asterisk. Настройка Asterisk для локальных звонков.

## Задание

1. Установить систему server.
   
2. Установить Asterisk.
   
3. Установить soft телефон на рабочую станцию.
   
4. Настроить SIP каналы.

5. Подключиться к SIP каналам soft телефона.

6. Сделать тестовый звонок на номер 1000
   
## Ход выполнения работы 

### Установка и настройка Asterisk

Установим Asterisk

![image](https://github.com/16Angeles/2024_2025-ip-telephony_k34202_islamov_s_s/blob/49f21e78604d0f1165cfba951dec0f5fb91b244a/lab3/1.png)


Редактируем файлы конфигурации

`sip.conf`

![Снимок экрана от 2025-03-12 14-34-37](https://github.com/user-attachments/assets/df302f7a-a656-4d3b-be03-261930a9bf04)

`extensions.conf`

![Снимок экрана от 2025-03-12 14-29-00](https://github.com/user-attachments/assets/6263d155-bf6e-4cf8-8f6d-8edc9903060b)

Перезапускаем службу с помощью sudo service asterisk restart

Проверяем, что все работает

![image](https://github.com/16Angeles/2024_2025-ip-telephony_k34202_islamov_s_s/blob/dce906f0b4e2046fa6d8b598cde6b52fa356e9bc/lab3/2.png)

### Установка и настройка телефона Zoiper

Скачиваем ZoiPer5 с официального сайта и распаковываем его

![image](https://github.com/16Angeles/2024_2025-ip-telephony_k34202_islamov_s_s/blob/731511f053635abd25754d15452133cf866ed67a/lab3/3.png)

Заходим в приложение под логином и паролем одного из созданных аккаунтов 

![Снимок экрана от 2025-02-19 17-02-27](https://github.com/user-attachments/assets/c543cfc2-e4e2-4106-a211-fced194ec441)

Проверим, что порт отображается внутри Asterisk

![image](https://github.com/16Angeles/2024_2025-ip-telephony_k34202_islamov_s_s/blob/a7bceff75f0ecc937cb9a244de2ca5b73ce44160/lab3/4.png)


### Установка и настройка MicroSIP

Cледуя инструкциям завершаем установку

![Снимок экрана от 2025-03-12 14-15-12](https://github.com/user-attachments/assets/0bd512fb-f01c-441f-9d7d-ead0c70b6cde)

Входим в ранее созданный аккаунт 

![Снимок экрана от 2025-03-12 14-18-10](https://github.com/user-attachments/assets/452f0b70-ea44-4adc-93fa-797a411edfdc)

Получаем следующий вид двух телефонов:

![Снимок экрана от 2025-03-12 14-18-46](https://github.com/user-attachments/assets/62a15a80-f56f-4fd5-b06f-77f8a2193679)

Проверим, что порты отображаются корректно:

![Снимок экрана от 2025-03-12 14-20-06](https://github.com/user-attachments/assets/2c0dd0cf-b2fc-4fd7-b819-b19db4959bcf)

Проверим сетевую связность:

`111 -> 222`

![Снимок экрана от 2025-03-12 14-36-34](https://github.com/user-attachments/assets/49506eea-93d3-4b21-9acf-c85507f792c9)

`222 -> 111`

![Снимок экрана от 2025-03-12 14-36-20](https://github.com/user-attachments/assets/56214d9e-c6dc-4e41-acb3-17b019eacf1e)

## Вывод 

В ходе выполнения работы был изучен и настроен для локальных звонков программный комплекс Asterisk. 



