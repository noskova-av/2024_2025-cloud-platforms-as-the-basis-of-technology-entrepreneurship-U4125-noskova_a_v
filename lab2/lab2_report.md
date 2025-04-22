<b>University:</b> [ITMO University](https://itmo.ru/ru/) <br>
<b>Faculty:</b> [FTMI](https://ftmi.itmo.ru) <br>
<b>Course:</b> [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) <br>
<b>Year:</b> 2024/2025 <br>
<b>Group:</b> U4125 <br>
<b>Author:</b> Noskova Alena Vyacheslavovna <br>
<b>Lab:</b> Lab2 <br>
<b>Date of create:</b> 22.04.2025 <br>
<b>Date of finished:</b> <br>

<h1>Отчет по лабораторной работе №2 </h1>
Описание заданий лабораторной работы можно найти здесь: https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/education/labs2023-2024/lab2/lab2/#_6

1. Создадим `Cloud Run` с минимальным количеством ресурсов из дефолтного сервиса Hello
![image](https://github.com/user-attachments/assets/5822bb63-6e59-4137-a8d2-71c050d12c1f)

2. Перейдем по ссылке, предоставленной `Cloud Run`
![image](https://github.com/user-attachments/assets/125ed197-f99d-4cc9-a587-61f917fcd621)

3. Сервис работает корректно
![image](https://github.com/user-attachments/assets/19038efc-1d88-4a83-945e-c357be48fdb4)

4. Перейдем в раздел `Logs`, проанализируем их
![image](https://github.com/user-attachments/assets/27436126-29ef-473b-b683-f24eb8acf31b)

5. Перейдем в раздел `Metrics`, проанализируем их
![image](https://github.com/user-attachments/assets/74278306-2b1a-41bf-a51f-aca2f8a4d77e)

6. Поменяем порт на 8090 для нашего `Cloud Run`. Для этого нажмем на кнопку `Edit & deploy new revision` и заменим значение порта.
![image](https://github.com/user-attachments/assets/c5861bee-8070-49a2-b6a5-46340faeffba)
![image](https://github.com/user-attachments/assets/93078043-01be-47b3-9e71-dd3bc541a458)

7. Отследим изменение метрик
![image](https://github.com/user-attachments/assets/d5df779f-8bb1-45ae-bf3d-7316462d37f4)

8. Переключим трафик между версиями. Для этого вернемся в раздел `Revisions`, откроем контекстное меню `Actions` и выберем пункт `Manage traffic`.
![image](https://github.com/user-attachments/assets/e3986ced-9514-4bd6-a63e-5363f6dded1a)

9. Зададим следующие параметры. Сохраним введенные значения.
![image](https://github.com/user-attachments/assets/8031e8ab-05a2-4a5d-a553-bbc6ec04d6b6)

10. Отследим изменение метрик
![image](https://github.com/user-attachments/assets/9625ddc4-fafc-4687-939d-4c04dee6c197)

11. Удалим все созданные сервисы.
