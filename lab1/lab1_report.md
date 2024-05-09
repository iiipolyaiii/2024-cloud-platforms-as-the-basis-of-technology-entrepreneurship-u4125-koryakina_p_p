University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FTMI](https://ftmi.itmo.ru)\
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/education/labs2023-2024/lab1/lab1/)\
Year: 2024\
Group: U4125\
Author: Koryakina Polina\
Lab: Lab1\
Date of create: 19.04.2024\
Date of finished: 19.04.2024


1) В разделе Identity and Access Management (IAM) мы создали Service Account с правами Storage Admin (широкий функционал)
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/412f785f-339a-46d4-81ee-75aeac842e20)
2) В разделе Computer Engine мы создали и запустили виртуальную машину, привязав ее к Service Account, который был создан в п.1
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/9a856f14-05c8-45a4-bad0-ba4cd668b076)
3) Идем в SSH ((Secure Shell, метод безопасного доступа и управления виртуальными машинами) и с помощью команды gsutil мы копируем файлы из бакета lab1-bucket-itmo. Далее с помощью команды ls -lah смотрим, что хранится в нашей ВМ
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/3e730a60-3fc7-4930-99de-512ed6b0505b)
4) Меняем роль Service Account с Storage Admin на Compute Viewer (роль с ограниченным доступом)
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/9eb3b862-56f8-4933-97e8-9ba1daefc096)
5) Снова, используя gsutil, пробуем скопировать фалы. У нас не получается это сделать, так как теперь Service Account, привязанный к ВМ, не обладает такими правами
![image](https://github.com/iiipolyaiii/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-koryakina_p_p/assets/164926981/72e3f2f7-73d2-4453-9204-7edfa287ebeb)

Таким образом, мы можем прийти к выводу о том, что в зависимости от настроек Service Account мы можем иметь различные права досупа, одни из которых открывают нам доступ к редактированию, в то время как другие позволяют только просматривать информацию

 
