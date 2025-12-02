# Отчет по лабораторной №1

University: [ITMO University](https://itmo.ru/ru/)\
Faculty: FTMI\
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)\
Year: 2025/2026\
Group: U4225\
Author: Barakhsin Grigorii Mikhailovich\
Lab: Lab1\
Date of create: 02.12.2025\
Date of finished: 02.12.2025

1. Зайдите в вкладку IAM, создайте service account с ролью Storage Admin\
![creation.png](creation.png)
![creation2](creation2.png)
2. Создать минимальный compute engine (виртуальную машину) с Machine type e2-micro в режиме spot.\
![](vm1.png)
3. С помощью утилиты gsutils найдите бакет lab1-bucket-itmo и скопируйте 3 файла в локальную папку на VM.\
Используя команду ls -lah отобразите что эти файлы хранятся у вас на VM.\
![](vm_out.png)
4. Поменяйте права доступа для вашего service account с Storage Admin на Compute Viewer, \
попробуйте повторить пункт с копированием данных, сделать выводы.
![img_7.png](role_change.png)
![img_8.png](role_change_result.png)
5. Выводы таковы, что при изменении уровня доступа меняются права и не все действия можно сделать.