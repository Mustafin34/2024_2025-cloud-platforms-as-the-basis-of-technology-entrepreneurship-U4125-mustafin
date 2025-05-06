University: [ITMO University](https://itmo.ru/ru/)
 Faculty: [FICT](https://fict.itmo.ru)
 Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)
 Year: 2024/2025
 Group: U4125
 Author: Mustafin Daniil Eduardovic
 Lab: Lab4
 Date of create: 04.05.2025
 Date of finished: .2025
# Лабораторная работа №4 "Разработка инфраструктуры MVP AI приложения."

## Описание:
Это четвертая лабораторная работа "Разработка инфраструктуры MVP AI приложения."

## Цель работы:
Создать прототип AI-приложения с базовой функциональностью.

## Ход работы:
### Основная функциональность:
1. Анализ настроения текста: Пользователь может вводить текстовые сообщения, статьи, отзывы или любой другой текст в приложение, и AI-модель будет анализировать этот текст и определять его настроение (положительное, отрицательное или нейтральное).
2. Визуализация результатов: После анализа приложение предоставляет пользователю визуализацию результатов в виде графиков или диаграмм, показывающих распределение настроения в тексте.
3. История анализов: Приложение сохраняет историю анализов пользователя, позволяя просматривать предыдущие результаты и сравнивать их.

### Инфраструктура приложения:
1. Frontend-сервер
2. Backend-сервер
3. База данных
4. NLP-модуль

### Структура:
<img width="1012" alt="Снимок экрана 2025-05-06 в 15 56 12" src="https://github.com/user-attachments/assets/58a3dd6f-99dc-4983-816a-bb58e0e0cec3" />

### Расчет стоимости развертывания системы:

**Test**

1. MongoDB - M10, 10GB storage, 1.7GB RAM - 57$/месяц
2. NLP - syntax + sentiment analysis, <1M символов - 0.0015$/1000 символов
3. Frontend App - B2 instance, 768mb, 1.2GHz - 83$/месяц
4. Microservices - F1 instance (x2), 384mb, 600MHz - 83$/месяц
5. Redis - M1, 1GB - 46$/месяц

**ИТОГО: 270.5$/месяц**

**Pre-prod**

1. MongoDB - M40, 80GB storage, 16GB RAM - 619$/месяц
2. NLP - syntax + sentiment analysis, <5M символов - 0.00225$/1000 символов
3. Frontend App - B2 instance, 768mb, 1.2GHz - 83$/месяц
4. Microservices - F1 instance (x2), 384mb, 600MHz - 83$/месяц
5. Redis - M1, 1GB - 46$/месяц

**ИТОГО: 842.25$/месяц**

**Prod**

1. MongoDB - M80, 750GB storage, 128GB RAM - 4413$/месяц
2. NLP - syntax + sentiment analysis, 5M+ символов - 0.001875$/1000 символов
3. Frontend App - B2 instance, 768mb, 1.2GHz - 83$/месяц
4. Microservices - F1 instance (x2), 384mb, 600MHz - 83$/месяц
5. Redis - M1, 1GB - 46$/месяц

**ИТОГО: 4643.75$/месяц (10M символов в запросах)**

## Вывод:
Познакомились со способами прототипирования веб сервисов и рассчета стоимости их реализации
