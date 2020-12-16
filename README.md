# LR6
Лабораторная работа №6
Цель лабораторной работы: 
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.  

## Ход работы:  

### 1. Настройка клиент git  
Вводим имя пользователя - "Lebedev E.M. 4918" и и email - egorkabofabo82.g@mail.com 

![шаг 1](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/1.jpg)  

### 2. Клонирование удалённого репозитория на компьютер  
Клонируем репозиторий 

![шаг 2](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/2.jpg)

### 3. Добавление файла через интерфейс GitHub  
Переходим в директорию и добавляем файл Egor.txt через интерфейс GitHub. Подтягиваем изменения в локальный репозиторий.  

![шаг 3](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/3.jpg)

### 4. Получение всей истории операций  

Получаем историю операций для каждой ветки:

master:

![шаг 4](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/4.jpg)

branch1:

![шаг 4](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/5.jpg)

Последние изменения:

![шаг 4](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/6.jpg)

### 6. Слияние в ветку master  

Выполняем слияние ветки branch1 в ветку master, разрешив конфликт c помощью графического интерфейса git.
При попытки слияния происходит конфликт

![шаг 6](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/7.jpg) 

Разрешение конфликта:

![шаг 6](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/8.jpg) 

![шаг 6](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/9.jpg) 

![шаг 6](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/10.jpg)

![шаг 6](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/11.jpg)
### 7. Удаление побочной ветки  
Удаляем побочную ветку после успешного слияния.

![шаг 7](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/12.jpg) 

### 8. Фиксирование изменений  

Делаем изменения в файле Ivan.txt и зафиксируем их, оставляя комментарии.  

![шаг 8](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/13.jpg)  

### 9. Откат коммита  

Делаем «хард» откат коммита.  

![шаг 9](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/14.jpg)  

### 10. Создание ветки  

Создаем ветку report для отчёта.   

![шаг10](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/15.jpg)

## Логи команд:  

/*Настройка клиента git и клонирование рперезитория*/

* git config --global user.name "Lebedev E.M. 4918"
* git config --global user.email egorkabofabo82@gmail.com
* git clone https://github.com/eradecator292/LR6.git
* cd LR6   
  
/*Добавление файл Egor.txt через интерфейс GitHub, получение истории операций для каждой из веток, просмотр последних изменений*/

* git pull  
* git log  
* git log -2  
* git checkout branch1  
* git checkout master  
* git merge branch1  
  
/*Cлияние в ветку master*/

* git checkout branch1  
* git checkout master  
* git merge branch1      

/*Удаление ветки branch1

* git branch -d branch1
    
/*изменение в файле Egor.txt*/   
   
* git add Ivan.txt  
* git commit -m "change 1"  

/* Хард откат коммита*/

* git reset --hard @~2  

/*Созадние ветки для отчёта*/

* git branch report

/*История операций в форматированном виде*/
* git log --pretty=format:"%h - %an, %ar : %s"

/*Отправка в сетевое хранилище*/
* git push https://github.com/eradecator292/LR6.git


## История операций:  

![история операций](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/16.jpg)  

## Отправка локальных изменений в сетевое хранилище GitHub:  

![отправка изменений](https://github.com/eradecator292/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/17.jpg)

### Вывод:
Я изучил базовые возможности системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.  
