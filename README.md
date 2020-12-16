# LR6
Лабораторная работа №6
Цель лабораторной работы: изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.  
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
![шаг 6](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/7.jpg) 
![шаг 6](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/8.jpg) 
![шаг 6](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/9.jpg) 
![шаг 6](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/10.jpg)
### 7. Удаление побочной ветки  
Удаляем побочную ветку после успешного слияния.
![шаг 7](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/12.jpg) 
### 8. Фиксирование изменений  
Делаем изменения в файле Ivan.txt и зафиксируем их, оставляя комментарии.  
![шаг 8](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/14.jpg)  
![шаг 8](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/13.jpg) 
### 9. Откат коммита  
Делаем «хард» откат коммита.  
![шаг 9](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/15.jpg)  
### 10. Создание ветки  
Создаем ветку report для отчёта.   
![шаг10](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/16.jpg )


## Логи команд:  
*  git config --global user.name "4918 Sinenok I.V."
* git config --global user.email sinenok.10@mail.ru
* git clone https://github.com/Sinenok-star/LR6.git
* cd LR6   
  
  
/*Добавление файл Ivan.txt через интерфейс GitHub*/
  
* git pull  
* git log  
* git log -2  
* git checkout branch1  
* git checkout master  
* git merge branch1  
  
/*Устранение конфликта в git GUI*/
    
* git branch -d branch   
    
 /изменение в файле Ivan /   
   
* git add Ivan.txt  
* git commit -m "change 1"  
* git reset --hard @~2  
* git branch report
## История операций:  
![история операций](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/17.jpg)  
## Отправка локальных изменений в сетевое хранилище GitHub:  
![отправка изменений](https://github.com/Sinenok-star/LR6/blob/report/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD/18.jpg)
Вывод:я изучил базовые возможности системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.  
