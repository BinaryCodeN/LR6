ГУАП
КАФЕДРА № 44
ОТЧЕТ 
ЗАЩИЩЕН С ОЦЕНКОЙ
ПРЕПОДАВАТЕЛЬ
ассистент



Т.Р. Мустафин
должность, уч. степень, звание

подпись, дата

инициалы, фамилия

ОТЧЕТ О ЛАБОРАТОРНОЙ РАБОТЕ №6

СИСТЕМА КОНТРОЛЯ ВЕРСИЙ

по курсу: ОСНОВЫ ПРОГРАММИРОВАНИЯ


РАБОТУ ВЫПОЛНИЛ
СТУДЕНТ гр. №
4217



А.Н. Медянкина



подпись, дата

инициалы, фамилия




Санкт-Петербург 
2023


ЦЕЛЬ РАБОТЫ
     Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.
     
ХОД РАБОТЫ
     Первым делом, для выполнения данной работы, нужно было создать аккаунт на Git Hub, но мне не пришлось его создавать, так как он у меня уже был.

Рисунок 1 – Аккаунт на платформе Git Hub
	Для клонирования репозитория LR6 в интерфейсе Git Hub был использован fork из аккаунта преподавателя в мой аккаунт BinaryCodeN.

Рисунок 2 – Создание копии другого репозитория в личном хранилище
	С помощью команды git –version была проверена установка программы Git.

Рисунок 3 – Установка Git на ноутбук
     Чтобы установки настроить клиент git, были использованы следующие команды: 
     git config –global user.name "Группа 4217 Медянкина А.Н."
     git config --global user.email nensijw3@gmail.com

Рисунок 4 – Настройки клиента git
     Клонирование репозитория осуществлялось путем использования команды git clone + [ссылка на репозиторий].

Рисунок 5 – Клонирование репозитория
     Через интерфейс Git Hub в репозиторий был добавлен новый файл New_file.txt.

Рисунок 6 – Добавлен новый файл
     Далее, использовав команду git pull origin master была получена история операций для каждой из веток, то есть для ветки master. 

Рисунок 7 – Подтягивание изменения в локальный репозиторий.
     Чтобы просмотреть коммиты и последние изменения в репозитории, использовалась команда git log.

Рисунок 8 –Все коммиты, сделанные в репозитории
	Для создания коммита файла mergefile.txt в ветке, была прописана следующая команда: git add mergefile.txt, git commit -m " ".

Рисунок 9 – создание коммита файла в новой ветке

     Далее, чтобы слить две ветки, а точнее new_branch поместить (слить) в master, использовалась следующий ряд команд: 
     git checkout master
     git merge new_branch

Рисунок 10 – Слияние двух веток
     После осуществления слияния ветки new_branch в master, нужно было удалить ненужную пустую ветку. Для этого была применена команда 
git branch -d new_branch

Рисунок 11 – Удаление побочной ветки
Добавление информации вручную в файл New_file.txt.
 
Рисунок 12 – Добавление информации в файл New_file.txt
     Чтобы отразить изменения в репозитории, в консоли был создан коммит с помощью команды git commit -m.

Рисунок 13 – Добавление информации в файл New_file.txt в консоли
Очередное добавление информации вручную в файл New_file.txt.

Рисунок 14 – Повторное добавление информации в файл New_file.txt 
     Чтобы еще раз отразить изменения в репозитории, в консоли был создан коммит с помощью команды git commit -m. Все изменения были зафиксированы.

Рисунок 15 – добавление информации в файл New_file.txt
     После завершения основных этапов в работе, следующим этапом нужно сделать откат коммита. Это можно сделать при помощи команды.
git revert HEAD

Рисунок 16 – Откат коммита

Рисунок 17 – Интерфейс в режиме HEAD 
     В качестве ветки для отчета, была создана ветка под названием task при помощи команды git branch task.

Рисунок 18 – Создание ветки для отчёта
     Чтобы получить историю операций в форматированном виде (сокращённый хэш + дата + имя автора + комментарий), была использована следующая команда: C:\Users\nensi\LR6>git log --pretty=format:"%h + %an + %an + %s".

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
