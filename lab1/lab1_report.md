University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)
Year: 2024/2025
Group: U4125
Author: Mustafin Daniil Eduardovic
Lab: Lab1
Date of create: 21.04.2025
Date of finished: .04.2025

# Лабораторная работа №1 "Обзор Google Cloud и исследование основных сервисов."

## Описание
Первая лабораторная работа "Обзор Google Cloud и исследование основных сервисов."

## Цель работы
Ознакомиться с основными возможностями и преимуществами облачной платформы Google Cloud.

## Ход работы

### 1.Создание сервисного аккаунта
Создали service account с ролью Storage Admin.
<img width="896" alt="Снимок экрана 2025-04-21 в 22 32 12" src="https://github.com/user-attachments/assets/81e25e60-8e3b-41af-a04b-9ff582eb06c2" />

### 2.Создание виртуальной машины
Создали минимальный compute engine (виртуальную машину) с Machine type e2-micro в режиме spot.
<img width="936" alt="Снимок экрана 2025-04-21 в 22 35 35" src="https://github.com/user-attachments/assets/da4d32fc-0c7e-4e00-bfdc-7c8cafa85961" />

### 3.Копирование файлов с бакета
С помощью утилиты gsutils нашли бакет lab1-bucket-itmo и скопировали 3 файла в локальную папку на VM. Используя команду ls -lah отобразили что эти файлы хранятся у вас на VM.
<img width="683" alt="Снимок экрана 2025-04-21 в 21 12 21" src="https://github.com/user-attachments/assets/27b62753-4211-4d13-a35b-9657a4cf65eb" />

### 4.Смена роли для сервисного аккаунта
Поменяли права доступа для вашего service account с Storage Admin на Compute Viewer.
<img width="896" alt="Снимок экрана 2025-04-21 в 22 32 12" src="https://github.com/user-attachments/assets/6c6d905e-1844-468a-83cf-1b1ff4bdd2f0" />

### 5.Повторное копирование файлов с бакета
Повторили пункт 3.
<img width="1512" alt="Снимок экрана 2025-04-21 в 22 07 07" src="https://github.com/user-attachments/assets/a47c1b26-9b9e-4a44-9e6e-f1b5fee681bf" />
