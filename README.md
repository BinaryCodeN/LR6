ПРЕПОДАВАТЕЛЬ: Т.Р. Мустафин


ОТЧЕТ О ЛАБОРАТОРНОЙ РАБОТЕ №6

Тема: СИСТЕМА КОНТРОЛЯ ВЕРСИЙ


РАБОТУ ВЫПОЛНИЛА А.Н. Медянкина




ЦЕЛЬ РАБОТЫ
     Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.
     

ХОД РАБОТЫ
     Первым делом, для выполнения данной работы, нужно было создать аккаунт на Git Hub, но мне не пришлось его создавать, так как он у меня уже был.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20230538.png)
Рисунок 1 – Аккаунт на платформе Git Hub


	Для клонирования репозитория LR6 в интерфейсе Git Hub был использован fork из аккаунта преподавателя в мой аккаунт BinaryCodeN.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20232839.png)
Рисунок 2 – Создание копии другого репозитория в личном хранилище


	С помощью команды git –version была проверена установка программы Git.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20212257.png)
Рисунок 3 – Установка Git на ноутбук


     Чтобы установки настроить клиент git, были использованы следующие команды: 
     git config –global user.name "Группа 4217 Медянкина А.Н."

     git config --global user.email nensijw3@gmail.com

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20213649.png)	
Рисунок 4 – Настройки клиента git


     Клонирование репозитория осуществлялось путем использования команды git clone + [ссылка на репозиторий].

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20231223.png)
Рисунок 5 – Клонирование репозитория


     Через интерфейс Git Hub в репозиторий был добавлен новый файл New_file.txt.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20232839.png)
Рисунок 6 – Добавлен новый файл


     Далее, использовав команду git pull origin master была получена история операций для каждой из веток, то есть для ветки master. 

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20233949.png)
Рисунок 7 – Подтягивание изменения в локальный репозиторий.


     Чтобы просмотреть коммиты и последние изменения в репозитории, использовалась команда git log.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-09%20235302.png)
Рисунок 8 –Все коммиты, сделанные в репозитории.


	Для создания коммита файла mergefile.txt в ветке, была прописана следующая команда: git add mergefile.txt, git commit -m " ".


![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20004806.png)
Рисунок 9 – создание коммита файла в новой ветке


     Далее, чтобы слить две ветки, а точнее new_branch поместить (слить) в master, использовалась следующий ряд команд: 
     git checkout master
     git merge new_branch

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20005250.png)
Рисунок 10 – Слияние двух веток


     После осуществления слияния ветки new_branch в master, нужно было удалить ненужную пустую ветку. Для этого была применена команда 
git branch -d new_branch

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20005529.png)
Рисунок 11 – Удаление побочной ветки


Добавление информации вручную в файл New_file.txt.
 
![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20005908.png)
Рисунок 12 – Добавление информации в файл New_file.txt


     Чтобы отразить изменения в репозитории, в консоли был создан коммит с помощью команды git commit -m.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20010022.png)
Рисунок 13 – Добавление информации в файл New_file.txt в консоли


Очередное добавление информации вручную в файл New_file.txt.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20010521.png)
Рисунок 14 – Повторное добавление информации в файл New_file.txt


     Чтобы еще раз отразить изменения в репозитории, в консоли был создан коммит с помощью команды git commit -m. Все изменения были зафиксированы.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20010829.png)
Рисунок 15 – добавление информации в файл New_file.txt


     После завершения основных этапов в работе, следующим этапом нужно сделать откат коммита. Это можно сделать при помощи команды.
git revert HEAD

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20012643.png)
Рисунок 16 – Откат коммита

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20011741.png)
Рисунок 17 – Интерфейс в режиме HEAD


     В качестве ветки для отчета, была создана ветка под названием task при помощи команды git branch task.

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20012643.png)
Рисунок 18 – Создание ветки для отчёта


     Чтобы получить историю операций в форматированном виде (сокращённый хэш + дата + имя автора + комментарий), была использована следующая команда: C:\Users\nensi\LR6>git log --pretty=format:"%h + %an + %an + %s".

![] (https://github.com/BinaryCodeN/LR6/blob/master/Фото%20выполнения%20работы/Снимок%20экрана%202023-11-10%20023727.png)
Рисунок 19 - Получение историю операций в форматированном виде


     Лог выполнения команд, прописанный в файле README.md:
C:\Users\nensi>git --version


C:\Users\nensi>git config --global user.name "Группа 4217 Медянкина А.Н."


C:\Users\nensi>git config --global user.email nensijw3@gmail.com


C:\Users\nensi>git init


C:\Users\nensi>git clone https://github.com/BinaryCodeN/LR6


C:\Users\nensi>git pull


C:\Users\nensi>dir


C:\Users\nensi>chdir LR6


C:\Users\nensi\LR6>git log


C:\Users\nensi\LR6>git branch new_branch


C:\Users\nensi\LR6>git chackout new_branch


C:\Users\nensi\LR6>git chackout new_branch mergefile.txt


C:\Users\nensi\LR6>git add mergefile.txt


C:\Users\nensi\LR6>git branch


C:\Users\nensi\LR6>git status


C:\Users\nensi\LR6>git add mergefile.txt


C:\Users\nensi\LR6>git commit -m "Файл с внесенными изменениями добавлен в новую ветку"


C:\Users\nensi\LR6>git branch


C:\Users\nensi\LR6>git checkout master


C:\Users\nensi\LR6>git merge new_branch


C:\Users\nensi\LR6>git branch -d new_branch


C:\Users\nensi\LR6>git add .


C:\Users\nensi\LR6>git commit -m "Добавление информации в New_file.txt"


C:\Users\nensi\LR6>git add .


C:\Users\nensi\LR6>git commit -m "Второй раз внесены очередные изменения в New_file.txt"


C:\Users\nensi\LR6>git reverte had


C:\Users\nensi\LR6>git revert HEAD


C:\Users\nensi\LR6>git branch task


C:\Users\nensi\LR6>git branch


C:\Users\nensi\LR6>git log --pretty=format:"%h + %an + %an + %s"


C:\Users\nensi\LR6>git add .


C:\Users\nensi\LR6>git commit -m "Итоговая версия"

C:\Users\nensi\LR6>git push origin master

Ссылка на репозиторий: https://github.com/BinaryCodeN/LR6/tree/master


ВЫВОД
     В процессе выполнения работы были изучены базовые возможности системы управления версиями, получены опыт работы с Git Api и с локальным и удаленным репозиторием.


