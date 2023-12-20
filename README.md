#О чём бот?

Бот помогает отслеживать все дедлайны, напоминает вам об их приближении. В боте представлена удобная сортировка дедлайнов по выставляемому приоритету. Помимо этого, можно вывести жизнерадостную и мотивирующую песенку, что является несомненно особенностью бота DeadBot.

Стартовая команда:
Для того, чтобы начать пользоваться ботом, введите /start

/start

Привет! DeadBot поможет расставить приоритеты твоих задач и собрать все дедлайны в одном месте.
Доступные команды:

/addDeadline - добавить дедлайн

/deleteDeadline - удалить дедлайн

/printDeadlines - вывести список дедлайнов

/changeDeadline - изменить характеристики дедлайна

/setReminder - установить напоминания

/printHappySong - вывести текст песни, которая поможет в трудную минуту

-В случае, если неверно введена команда на любом этапе выводится "Неверная команда. Попробуйте еще раз"

/addDeadLine

   Выберите дату дедлайна.
   
   /tommorow
   
   /setDate 13.10.2005
   
   -Если дата введена неверно выводится "Неверно введена дата. Попробуйте еще раз"
   
      Добавьте название дедлайна
      
         Добавьте описание к дедлайну (необязательно)
         
         /noDescription - без описания
         
         /addDescription "text"
         
            Введите приоритет (от 0 до 10), где 10 - важно.
            
            -Если приоритет выбран неверно, выводится "Неверный приоритет. Попробуйте еще раз"
            
   Успешно добавлен дедалйн "name" (description) с приоритетом priority.
   
После каждого успешного выполнения команды выводится:
Для перехода в меню напишите /back
   
/deleteDeadline

   -Если дедлайнов нет, выводится "Дедлайнов нет, вы счастливый человек :)"
   
   Выберите дедлайн из списка:
   
   1. dateOfDeadline firstDeadLine
   
   ....
   
      -Если неверно введен номер, выводится "Введен неверный номер. Попробуйте еще раз"
   Дедлайн успешно удален.
   

/printDeadlines

   1. dateOfDeadline nameOfFisrtDeadline (description) приоритет - priority.
   
/printHappySong - выводит текст песни pyrokinesis дедлайны

/changeDeadline

   -Если дедлайнов нет, выводится "Дедлайнов нет, можете спать спокойно"
   
   Выберите дедлайн:
   
   1. dateOfDeadline firstDeadLine
   
   ....
   
      Что вы хотите изменить?
      
       /changeDate
       
          Введите дату в формате 13.10.2005
          
          -Если дата введена неверно, выводится "Неверно введена дата. Попробуйте еще раз"
          
          Дата успешно изменена. Не откладывайте выполнение дела на потом!
          
       /changePriority
       
          Введите приоритет от 0 до 10.
          
          -Если приоритет выбран неверно, выводится "Неверный приоритет. Попробуйте еще раз"
          
          Приоритет успешно изменен.
          
       /changeDescription
       
          Введите описание
          
          Описание успешно изменено.
          
       /changeName
       
          Введите новое имя дедлайна.
          
          Название успешно изменено.
          
 /setReminder
 
    -Если дедлайнов нет, выводится "No deadlines"
    
    На сколько дедлайнов вы хотите установить напоминание?
    
    /all - на все дедлайны
    
    /one - на один дедлайн
    
       Для ветки /one:
       
          Выберите дедлайн:
          
          1. dateOfDeadline firstDeadLine
          
          ....
          
       Для всех веток:
       
          Как часто вы хотите получать напоминания?
          
          /everyDay - каждый день
          
          /everyWeek - каждую неделю
          
          /setFrequency - установить частоту напоминаний
          
          Для /setFrequency:
          
          Введите число (раз в сколько часов присылать уведомление)
          
          -Если введено неверное число, то выводится "Неверное количество часов. Try again"
          
          Для /one:
          
          Теперь вы будете получать уведомления для дедлайна DeadlineName раз в h часов/день/неделю
          
          Для /all:
          
          Теперь вы будете получать уведомления раз в h часов/день/неделю
          
 Шаблон напоминания: 
Привет! Это DeadBot. Самое время вспомнить о надвигающихся дедлайнах, а именно об "название дедлайна"! Дедлайн - "дата дедлайна".
          
Вывод команды /printHappySong:
[Текст песни «Дедлайны»]

[Куплет]
Ни один вопрос, увы, не решён
И за окнами прячемся от мира, как за решётками
В облаках перелётные птицы снова споют обреченно
Сонату о том, что всё когда-то становится чёрным
А белые полосы на шоссе, как разделительный знак
И там где закат и рассвет — мы застряли
Между двух дорог и за дверью ворот не нашли ничего
Что нити жизни сможет сплести в узелок опять!
И нас рвёт на куски
И я старался не теряться, но пропал, ты прости
Моя тропа позади, и я слетел на обочину
Ведь смотрел в пустоту так долго и сосредоточенно
Извини, времени нет, времени мало, время пропало
И всё, всё время идёт не по плану
Время диктует закон и время стирает в песок
И время лишь обещает, но сделать лучше никак не смогло
Орём, что нам плевать, но ускорясь
Мы делаем всё для того, чтобы запрыгнуть в горящий поезд
Да лишь не умереть бы никем и не стать нелюбимым
Но каждый миг в этом мире, как будто сталь гильотины
Холод металла, целующий плечи
И жизни клинок беспощаден и так безупречен
И прошу, времени хоть немного отдай мне
И я молод, но так давят отовсюду дедлайны
Но почему?
[Предприпев]
Когда придёт успех — я не знаю, но подожду
Когда я полюблю — я не знаю, но подожду
Когда я всё пойму — я не знаю, но подожду
И когда я умру — не знаю, но всё-таки подожду

[Припев]
Когда же ты раскроешь все тайны?
Я прошу, передвинь немного стрелочку таймера
А только шум от часов не даёт всё продумать детально
Всё сложнее писать и меня так давят дедлайны!
Но подожду, когда же ты раскроешь все тайны
И я прошу, передвинь немного стрелочку таймера
А только шум от часов не даёт всё продумать детально
Всё сложнее писать и меня так давят дедлайны
Но подожду, когда же ты раскроешь все тайны
Передвинь немного стрелочку таймера
Только шум от часов не даёт всё продумать детально
Всё сложнее писать и меня так давят дедлайны

[Постприпев]
Но подожду
Когда придёт успех — я не знаю, но подожду
Когда я полюблю — я не знаю, но подожду
Когда я всё пойму — я не знаю, но подожду
И когда я умру — не знаю, но всё-таки подожду
[Бридж]
Нет ответа на столько вопросов, и
Привяжи меня тут самыми крепкими тросами
Меня уносит течение в никуда!
Я 20 лет живу, но то что ищу, нигде так и не видал!
Покажи мне, где взлётная полоса
Надо как-то жить, но прости меня, я устал
Останови этот мир на минутку и подай мне руку;
И не дай как им без конца утонуть тут никогда!
Нет ответа на столько вопросов, и
Привяжи меня тут самыми крепкими тросами
Меня уносит течение в никуда!
Я 20 лет живу, но то что ищу, нигде так и не видал!
Покажи мне, где взлётная полоса
Надо как-то жить, но прости меня, я устал
Останови этот мир на минутку и подай мне руку
И не дай как им без конца утонуть тут никогда!
Через переулки, кварталы по городам
Как в той самой песне, разбившейся пополам
Мой голос вновь пролетает меж мокрых крыш
Разнеся, будто звук отчаянья
Эту песню ты слышишь, где-то там
Через переулки, кварталы по городам
Как в той самой песне, разбившейся пополам
Мой голос вновь пролетает меж мокрых крыш
Разнеся, будто звук отчаянья — эту песню ты слышишь...
И нет ответа на столько вопросов, и
Привяжи меня тут самыми крепкими тросами
Меня уносит течение в никуда!
Я 20 лет живу, но то что ищу, нигде так и не видал!
Через переулки, кварталы по городам
Как в той самой песне, разбившейся пополам
Мой голос вновь пролетает меж мокрых крыш
Разнеся, будто звук отчаянья — эту песню ты слышишь...
Покажи мне, где взлётная полоса
Надо как-то жить, но прости меня, я устал
Останови этот мир на минутку и подай мне руку;
И не дай как им без конца утонуть тут, и тогда
Через переулки, кварталы по городам
Как в той самой песне, разбившейся пополам
Мой голос вновь пролетает меж мокрых крыш
Разнеся, будто звук отчаянья — эту песню ты слышишь...
[Припев]
Когда же ты раскроешь все тайны?
Я прошу, передвинь немного стрелочку таймера
Только шум от часов не даёт всё продумать детально
Всё сложнее писать и меня так давят дедлайны!

[Аутро]
Но подожду...
Когда придёт успех — я не знаю, но подожду
Когда я полюблю — я не знаю, но подожду
Когда я всё пойму — я не знаю, но подожду
И когда я умру — не знаю, но всё-таки подожду
