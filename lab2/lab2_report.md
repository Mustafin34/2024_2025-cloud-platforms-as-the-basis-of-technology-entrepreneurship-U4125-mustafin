University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)
Year: 2024/2025
Group: U4125
Author: Mustafin Daniil Eduardovic
Lab: Lab1
Date of create: 3.05.2025
Date of finished: .2025

# Лабораторная работа №2 "Исследование Cloud Run"

## Описание
Это вторая лабораторная работа "Исследование Cloud Run".

## Цель работы
Ознакомиться с работой Cloud Run.

## Ход работы
### 1.Создание Cloud Run из представленного дефолтного сервиса Hello с минимальным количеством ресурсов.

<img width="1188" alt="Снимок экрана 2025-05-03 в 21 07 37" src="https://github.com/user-attachments/assets/7cf0fd41-b08e-4ce5-a533-ec5dbf006e1f" />
<img width="1186" alt="Снимок экрана 2025-05-03 в 21 07 56" src="https://github.com/user-attachments/assets/937dd9ec-af6e-48eb-8867-bffa0c9ea203" />
<img width="1185" alt="Снимок экрана 2025-05-03 в 21 08 19" src="https://github.com/user-attachments/assets/288a776b-6e95-4fd7-8bcc-2638764cb3d9" />

### 2.Переход к  Cloud Run, тестирование сервиса.

<img width="913" alt="Снимок экрана 2025-05-03 в 21 12 34" src="https://github.com/user-attachments/assets/ee85493e-3f9d-45f9-84c6-24fd05b486f2" />

### 3.Переход в разделы логи и метрики, анализ.

<img width="1510" alt="Снимок экрана 2025-05-03 в 21 14 06" src="https://github.com/user-attachments/assets/e220a74f-dec8-4745-a281-e3398c03bdf2" />
<img width="1493" alt="Снимок экрана 2025-05-03 в 21 17 27" src="https://github.com/user-attachments/assets/aa64b317-bb3c-4d1d-8a59-0717e0fc75de" />
<img width="1479" alt="Снимок экрана 2025-05-03 в 21 17 39" src="https://github.com/user-attachments/assets/8666efbd-f79b-4d54-ab28-272347346730" />
<img width="1481" alt="Снимок экрана 2025-05-03 в 21 17 49" src="https://github.com/user-attachments/assets/386acf39-47af-4989-9f7e-097f6ec07f42" />

### 4.Изменение Cloud Run, поменяв порт на 8090. Переключение трафика между версиями.

<img width="1504" alt="Снимок экрана 2025-05-03 в 21 21 49" src="https://github.com/user-attachments/assets/262b4f8d-694a-46cd-acbb-93ef5331b6e7" />
<img width="1512" alt="Снимок экрана 2025-05-03 в 21 23 48" src="https://github.com/user-attachments/assets/f936cf26-2fce-4f8a-83f5-9f690b636ae5" />
<img width="1508" alt="Снимок экрана 2025-05-03 в 21 24 45" src="https://github.com/user-attachments/assets/0107498c-ba78-489d-a969-ef49be4f0df6" />
<img width="1487" alt="Снимок экрана 2025-05-03 в 21 25 01" src="https://github.com/user-attachments/assets/6e436a2f-32e2-4e10-b61a-0719fd0153c3" />
<img width="1490" alt="Снимок экрана 2025-05-03 в 21 25 11" src="https://github.com/user-attachments/assets/70d8d392-d735-4ecd-9a4f-331a57e848d5" />

### 5.Удаление за собой всех созданных сервисов.

## Выводы
- В логах видно, что контейнер теперь запускается и слушает порт 8090 вместо 8080.
- Произошло обновление сервиса (ReplaceService), после чего контейнер выводит сообщение о старте на новом порту.
- Container Instance Count: наблюдался всплеск до двух активных экземпляров во время переключения.
- CPU/Memory Utilization: минимальные нагрузки, стабильные показатели (CPU около 1%, память около 10-20%).
- Container Startup Latency: небольшая задержка старта контейнера (примерно 80 мс).
- Max Concurrent Requests: максимум 2 одновременных запроса во время переключения.
