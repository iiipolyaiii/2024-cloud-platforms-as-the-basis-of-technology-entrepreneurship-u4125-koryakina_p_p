University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FTMI](https://ftmi.itmo.ru)\
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/education/labs2023-2024/lab1/lab1/)\
Year: 2024\
Group: U4125\
Author: Koryakina Polina\
Lab: Lab1\
Date of create: 19.04.2024\
Date of finished: 


1) Создаем Cloud Run из представленного дефолтного сервиса Hello
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/1ba23ae7-0bcd-4486-b564-d135dddb7163)
2) После того как Cloud Run создан, заходим в него, переходим по ссылке и оказываемся на стричке, где содержится имя, которое мы укахали при создании
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/82c8329a-a7dc-438a-867d-082b9176ac37)
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/6344eafd-6340-4759-bd70-47707a796117)
3) Создаем некоторую активность на страничке, после чего переходим обратно в Google Cloud и заходим во вкладки LOGS и METRICS. На вкладке LOGS мы видим, что происходило при развертывании CLoud Run
В предпоследнем, к примеру, видим, что контейнер успешно запущен и готов принимать HTTP запросы
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/ac29539c-b307-4ccd-b6fe-69cf76724303)
На вкладке METRICS мы можем видеть как менялись во времени различные метрики. Такие как Request count (Number of requests reaching the service), Container instance count (Number of container instances that exist for the service) и другие
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/81ab15d9-3730-467e-b01d-1b507e1eba08)
4) Меняем Cloud Run, поменяв порт на 8090. На странице, которая отображается по ссылке изменилось название (с 1 на 2)
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/cdd8a690-aba4-47be-8ab0-13a82bcb2c2c)
5) Перевключаемся между версиями и смотрим, как это отражается в метриках
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/953d1510-d5f4-4ca3-b722-08c3e53c52a0)
Изменения явно отражаются на графиках (сами графики можно менять с точки зрения визуализации данных) 
 ![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/56f377bb-d2f6-40e7-89ce-b02bf4bbb002)
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/de0698e8-fee7-4d8e-b992-c9f9e59eb6fb)
Итог: С помощью CLoud Run мы можем запускать контейнеры и следить за различными метриками, которые отражают уровень нагрузки и т.д. 
