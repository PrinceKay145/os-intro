# Отчёт о выполнении лабораторной работы №1 Установка и конфигурация операционной системы на виртуальную машину
***Российский Университет Дружбы Народов***  
***Факульткт Физико-Математических и Естественных Наук***  

 ***Дисциплина:*** *Операционные системы*  
 
 ***Работу выполнял:*** *Адебайо Ридван*
  *1032205020*  
 
 *НКНбд-01-20*  
 
 ***Москва. Дисплейный класс РУДН. 2021г.*** 
 
# Цель работы
Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для
дальнейшей работы сервисов.

# Задание
Установить и настроить для дальнейшей работы виртуальную машину Linux

# Выполнение лабораторной работы
1.	Я установил на личный компьютер Oracle Virtual Machine  
	![Oracle VM](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/1.jpg)
2. Настраиваю VM для установки Linux CentOS  
	- Указываю имя виртуальной машины и тип гостевой ОС  
	![Имя ВМ и тип ОС](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/002.jpg)
	- Создаю виртуальный диск типа VDI объемом 30 Гб  
	![Выбор типа диска](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/003.jpg)
3. Пошаговая установка и настройка CentOS  
	- В разделе "Выбор приложений" выбираем "Сервер с GUI"  
	![Выбор приложений](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/006.jpg)
	- Установка пароля администратора  
	![Установка пароля](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/010.jpg)
	- Отключаю KDUMP  
	![Отключение KDUMP](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/007.jpg)
	- Принимаем лицензионное соглашение  
	![Лицензионное соглашение](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/012.jpg)
4. Подключаю образ диска дополнений гостевой ОС  
![Установка образа](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/013.jpg)

# Домашнее задание
1. Анализирую последовательность загрузки системы с помощью команды ```dmesg | less```  
![dmesg в терминале](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw1.jpg)
2. Получаем необходимую информацию с помощью команды ```dmesg | grep -i "..."```  
    1. Версия ядра линукс  
    ![Linux Version](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw2.jpg)
    2. Частота процессора  
    ![Частота процессора](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw3.jpg)
    3. Модель процессора  
    ![Модель процессора](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw4.jpg)
    4. Объем доступной оперативной памяти  
    ![Объем доступной оперативной памяти](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw5.jpg)
    5. Тип обнаруженного гипервизора  
    ![Тип обнаруженного гипервизора](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw6.jpg)
    6. Тип файловой системы корневого раздела  
    ![Тип файловой системы корневого раздела](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw7.jpg)
    7. Последовательность монтирования файловых систем  
    ![Последовательность монтирования файловых систем](https://github.com/PrinceKay145/os-intro/blob/master/Lab01/image/nhw8.jpg)
   
# Выводы
Данная лабораторная работа помогла мне научиться устанавливать и использовать виртуальную машину для работы.
Я научился производить первоначальную настройку Oracle VM для работы с ОС CentOS.
Также я научился использовать команду ```dmesg``` для поиска нужной информации о системе.
