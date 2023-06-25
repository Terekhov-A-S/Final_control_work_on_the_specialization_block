# Итоговая контрольная работа по блоку специализация

![pictures for project](https://raw.githubusercontent.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/main/github-header-image.png)

## Урок 2. Итоговая контрольная работа

[ПЕРЕЙТИ К ЗАДАНИЮ](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block#задание)

[ПЕРЕЙТИ К РЕШЕНИЮ](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block#решение)

**Информация о проекте**

* Необходимо организовать систему учета для питомника в котором живут домашние и вьючные животные.


**Как сдавать проект**

Для сдачи проекта необходимо создать отдельный общедоступный репозиторий (Github, Gitlub или Bitbucket). 
Разработку вести в этом репозитории, использовать пул реквесты на изменения. Программа должна запускаться и работать, 
ошибок при выполнении программы быть не должно. Программа может использоваться в различных системах, поэтому необходимо
разработать класс в виде конструктора.


### Задание

1. Используя команду cat в терминале операционной системы Linux, создать два файла "Домашние животные"
(заполнив файл "собаками", "кошками", "хомяками") и "Вьючные животные" (заполнив файл "лошадьми", "верблюдами" и "ослами"), 
а затем объединить их. Просмотреть содержимое созданного файла. Переименовать файл, дав ему новое имя "Друзья человека".
2. Создать директорию, переместить файл туда.
3. Подключить дополнительный репозиторий MySQL. Установить любой пакет из этого репозитория.
4. Установить и удалить deb-пакет с помощью dpkg.
5. Выложить историю команд в терминале Ubuntu.
6. Нарисовать диаграмму, в которой есть классы - родительский, домашние животные и вьючные животные, 
в составы которых в случае домашних животных войдут классы: собаки, кошки, хомяки, а в класс вьючные животные войдут: 
лошади, верблюды и ослы.
7. В подключенном MySQL репозитории создать базу данных “Друзья человека”.
8. Создать таблицы с иерархией из диаграммы в БД.
9. Заполнить низкоуровневые таблицы именами (животных), командами которые они выполняют и датами рождения.
10. Удалить из таблицы верблюдов, т.к. верблюдов решили перевезти в другой питомник на зимовку. 
Объединить таблицы "лошади", и "ослы" в одну таблицу.
11. Создать новую таблицу "молодые животные" в которую попадут все животные старше 1 года, но младше 3 лет 
и в отдельном столбце, с точностью до месяца, подсчитать возраст животных в новой таблице.
12. Объединить все таблицы в одну, при этом сохраняя поля, указывающие на прошлую принадлежность к старым таблицам.
13. Создать класс с Инкапсуляцией методов и наследованием по диаграмме.
14. Написать программу, имитирующую работу реестра домашних животных.
    В программе должен быть реализован следующий функционал:

    14.1. Завести новое животное;

    14.2. Определять животное в правильный класс;

    14.3. Увидеть список команд, которое выполняет животное;

    14.4. Обучить животное новым командам;

    14.5. Реализовать навигацию по меню.

15. Создайте класс Счетчик, у которого есть метод add(), увеличивающий̆ значение внутренней̆ int переменной̆ на 1 
при нажатии “Завести новое животное”. Сделайте так, чтобы с объектом такого типа можно было работать в блоке try-with-resources. 
Нужно бросить исключение, если работа с объектом типа счетчик была не в ресурсном try и/или ресурс остался открыт. 
Значение считать в ресурсе try, если при заведения животного заполнены все поля.


### Решение

1. 
```
cat > "Домашние животные"
Собаки
Кошки
Хомяки

'Ctrl+d'
```

```
cat > "Вьючные животные"
Лошади
Верблюды
Ослы

'Ctrl+d'
```

```
cat "Домашние животные" "Вьючные животные" > Animals
cat Animals
mv "Animals" "Друзья человека"
```

![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/1_2.png)

2. 
```
mkdir folder_for_attestation
mv 'Друзья человека' folder_for_attestation/
ls
cd folder_for_attestation/
ls
```

![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/2.png)

3. 
```
cat > "Вьючные животные"
Лошади
Верблюды
Ослы

'Ctrl+d'
```

![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/3_1.png)
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/3_2.png)
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/3_3.png)
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/3_4.png)

4.
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/4_1.png)
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/4_2.png)

5.
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/5.png)

6.
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/diagram.png)

7.
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/7.png)

8.
![pictures for project](https://github.com/Terekhov-A-S/Final_control_work_on_the_specialization_block/blob/main/Source/8.png)

9.
10.
11.
12.
13.
14.
15.




*Подготовил студент Geek Brains* [**`Терехов Александр`**](https://gb.ru/users/7696463), Final_control_work_on_the_specialization_block
