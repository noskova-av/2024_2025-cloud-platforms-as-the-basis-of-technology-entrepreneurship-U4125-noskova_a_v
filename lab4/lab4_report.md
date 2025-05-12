<b>University:</b> [ITMO University](https://itmo.ru/ru/) <br>
<b>Faculty:</b> [FTMI](https://ftmi.itmo.ru) <br>
<b>Course:</b> [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) <br>
<b>Year:</b> 2024/2025 <br>
<b>Group:</b> U4125 <br>
<b>Author:</b> Noskova Alena Vyacheslavovna <br>
<b>Lab:</b> Lab4 <br>
<b>Date of create:</b> 10.05.2025 <br>
<b>Date of finished:</b> 12.05.2025<br>

<h1>Отчет по лабораторной работе №4 </h1>
Описание заданий лабораторной работы можно найти здесь: https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/education/labs2023-2024/lab4/lab4/

<h3>Описание сервиса</h3>
Сервис предназначен для предобработки отзывов посетителей ресторанов, использующих агрегатор для бронирования мест в заведениях. Анализируется общая тональность отзыва: наличие нецензурной лекции, его объем, ключевые слова.

Предполагается наличие трех контуров/состояний развития сервиса:
1. Начальный (dev)
2. Тестирование партнерами (test)
3. Продовое решение (prod)

<h2>Начальное решение</h2>
Развертывание и использование ведется командой разработки. Ведется разработка и тестирование участниками проектной команды. <br>
<br>

**Компоненты:** <br> 
<br>
•	Cloud Run: размещение API-сервиса, обрабатывающего запросы <br>
•	Cloud Storage: хранение предобученной модели <br>
•	Firestore: сохранение истории запросов и результатов анализа <br>
<br>

**Алгоритм работы:**
1.	Пользователь отправляет текстовый запрос к API в Cloud Run.
2.	Cloud Run вызывает модель из Cloud Storage.
3.	Модель анализирует текст и определяет его тональность.
4.	Результат сохраняется в Firestore.
5.	Ответ возвращается пользователю.

![image](https://github.com/user-attachments/assets/f056411f-a37b-46cd-9dee-eb92e73688f6)
<br>
**Стоимость решения в месяц:** <br>
<br>
![image](https://github.com/user-attachments/assets/2cf16e4a-35cc-4fb5-ae16-eae9ec546e28)

<br> 
<h2>Тестирование партнерами</h2>
На этом этапе сервис предоставляется ограниченному числу человек для тестирования. Требуется обеспечить масштабируемость и сбор аналитики.
<br>
<br>

**Компоненты:** <br> 
<br>
• Cloud Run: Обработка запросов и взаимодействие с моделью <br>
• Vertex AI Model: Централизованное хранение и управление версиями ML-модели <br>
• Cloud SQL: Хранение информации о пользователях и аналитических данных <br>
• Firestore: Логирование <br>
• Cloud Monitoring: Отслеживание метрик и ошибок <br>
<br>

**Алгоритм работы:**
1. Пользователь отправляет текстовый запрос на API, размещённый в Cloud Run.
2. Cloud Run загружает модель из Vertex AI и анализирует текст.
3. Результаты сохраняются в Cloud SQL и Firestore.
4. Все сервисы отправляют метрики и логи в Cloud Monitoring
5. Ответ возвращается пользователю.

![image](https://github.com/user-attachments/assets/32ead06f-f8f4-45f9-856f-ed6b7d5d6927)
<br>
**Стоимость решения в месяц:** <br>
<br>
![image](https://github.com/user-attachments/assets/c3bc85bd-c193-416f-8b2b-d527533b960f)

<br> 
<h2>Продовое решение</h2>
Ориентирование на увеличение нагрузки и роста числа пользователей.
<br>
<br>

**Компоненты:** <br> 
•	GKE (Google Kubernetes Engine): Размещение и управление контейнерами приложения <br> 
•	Vertex AI Model: Централизованное хранение и управление версиями ML модели <br> 
•	Cloud SQL: Хранение информации о пользователях и аналитических данных <br> 
•	Firestore: Сохранение логов <br> 
•	Cloud Monitoring: Отслеживание метрик и ошибок <br> 
<br> 

**Алгоритм работы:**
1.	Пользователь отправляет текстовый запрос на API, размещённый в Cloud Run.
2.	GKE загружает модель из Vertex AI и анализирует текст.
3.	Результаты сохраняются в Cloud SQL и Firestore.
4.	Все сервисы отправляют метрики и логи в Cloud Monitoring
5.	Ответ возвращается пользователю.

![image](https://github.com/user-attachments/assets/dc77e9bb-1a32-4797-a33e-289e423a1631)
<br>
**Стоимость решения в месяц:** <br>
<br>
![image](https://github.com/user-attachments/assets/78419b7f-0d92-4f5b-a985-535a686e5215)
