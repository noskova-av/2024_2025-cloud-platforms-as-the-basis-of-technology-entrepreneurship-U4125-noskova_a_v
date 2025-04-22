<b>University:</b> [ITMO University](https://itmo.ru/ru/) <br>
<b>Faculty:</b> [FTMI](https://ftmi.itmo.ru) <br>
<b>Course:</b> [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) <br>
<b>Year:</b> 2024/2025 <br>
<b>Group:</b> U4125 <br>
<b>Author:</b> Noskova Alena Vyacheslavovna <br>
<b>Lab:</b> Lab1 <br>
<b>Date of create:</b> 21.04.2025 <br>
<b>Date of finished:</b> 22.04.2025<br>

<h1>Отчет по лабораторной работе №1 </h1>
Описание заданий лабораторной работы можно найти здесь: https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/education/labs2023-2024/lab1/lab1/

1. Перейдем в раздел `IAM & Admin` на вкладку `Service Accounts`. Создадим сервисный аккаунт.
![image](https://github.com/user-attachments/assets/4c98cba8-157d-4faf-add6-b2e9d2c452e3)

2. Зададим нейминг аккаунта в соответствии с указанной в лабораторной маской. Перейдем к следующему шагу
![image](https://github.com/user-attachments/assets/2122b14c-8198-4938-9b8c-b4b7aa10c36e)

3. Выбираем роль `Storage Admin`. Сохраняем созданный аккаунт.
![image](https://github.com/user-attachments/assets/45dcca47-9d71-41c4-9446-26b8c192afa4)

4. Теперь создадим и настроим виртуальную машину. Для этого перейдем в раздел `Compute Engine` на вкладку `VM instances` и нажмем на кнопку `Create instance`.
![image](https://github.com/user-attachments/assets/240c1c9b-5ec8-4f7a-b6b0-e92b42fb27ef)

5. Создадим машину со следующими параметрами (_при корректной настройке стоимость должна быть равна $3.44_):
![image](https://github.com/user-attachments/assets/9e5f2ecd-5e0a-4f6c-a090-3f07156bedbc)
![image](https://github.com/user-attachments/assets/708887b6-d665-471a-8647-d239df2a3102)
![image](https://github.com/user-attachments/assets/5248210c-446b-4f07-9dd7-3aeba795cbba)

6. Подключимся к созданной машине по SSH
![image](https://github.com/user-attachments/assets/a4ef1515-2ce6-4bdc-8e0c-c58f8146958a)

7. В открывшемся окне введем команды для создания новой папки и копирования в нее заданных файлов. Закроем SSH-подключение.
![image](https://github.com/user-attachments/assets/a1e6b522-ceeb-4245-8964-b59e4f1b416b)

8. Вернемся в раздел `IAM & Admin` на вкладку `Service Accounts`. Зададим новую роль `Compute Viewer` для сервисного аккаунта.
![image](https://github.com/user-attachments/assets/ee9d23db-93d4-432e-91b3-69bdafa4f419)

9. Снова запустим SSH-подключение. При попытке перенести данные на ВМ выдает следующую ошибку из-за отсутствия небоходимых прав доступа:
![image](https://github.com/user-attachments/assets/50c8133b-56e0-4934-bbe8-7cb0ab745c71)

10. Удалим созданную ВМ и сервисный аккаунт.
