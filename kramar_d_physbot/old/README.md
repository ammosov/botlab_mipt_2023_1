# Сценарии бота

## Знакомство

-   $/start$ - Вас приветствует Physbot - бот для отслеживания ваших
    посещений по физической культуре. Введите ваш адрес электронной
    почты в домене \@phystech.edu, для сохранения ваших посещений в
    случае потери данных.

-   *ivanov.ii@phystech.edu* - Добро пожаловать в Physbot.
  Ваше текущее количество посещений: *0*.
  Ваша специализация: *ОФП (М)*.
  Дни недели: *Не указано*
  Доступные команды:

    1.  $/add$ - Добавить посещение

    2.  $/addSickLeave$ - Добавить больничный

    3.  $/addDays$ - Добавить дни недели с физкультурой

    4.  $/addSpecialisation$ - Добавить специализацию

    5.  $/profile$ - Показать профиль и количество посещений

    6.  $/calculateAttendance$ - Посчитать количество посещений в неделю для закрытия к определённой дате

    7.  $/list$ - Все ваши посещения

    8.  $/reminder$ - Включить или отключить напоминания

## Добавление посещения

-   $/add$ - На какой день вы хотите добавить посещение?

    1.  $/today$ - Сегодня

    2.  $/previous$ - На предыдущий по расписанию день

    3.  */select* - Выбрать дату

        -   */select 11.11.2023* - На 11 ноября 2023 года

-   $/addSickLeave$ - Два сценария: дни физкультуры добавлены или не
    добавлены.

    1.  **Дни физкультуры добавлены.** Ответ бота: Введите даты
        больничного с помощью команды /select вида */select
        01.11.2023 - 14.11.2023*.

    2.  **Дни физкультуры не добавлены**. Вызывается команда $/addDays$,
        а после её выполнения переход на $/addSickLeave$ с уже
        известными днями с физкультурой.

## Добавление свойств пользователя

-   $/addDays$ - Текущие дни недели: *Не указано*. Чтобы добавить дни
    напишите команду */select* вида */select пн ср чт*. Все дни недели:

    1.  пн - Понедельник

    2.  вт - Вторник

    3.  ср - Среда

    4.  чт - Четверг

    5.  пт - Пятница

    6.  сб - Суббота

    7.  вс - Воскресенье

-   $/addSpecialisation$ - Введите вашу специализацию в виде */select
    Баскетбол*

-   $/reminder$ - Вы включили/выключили напоминания по воскресеньям.

## Вывод посещений

-   $/profile$ - Добро пожаловать в Physbot. Ваше текущее количество
    посещений: *0*. Ваша специализация: *ОФП (М)*. Дни недели: *Не
    указано* Доступные команды:

    1.  $/add$ - Добавить посещение

    2.  $/addSickLeave$ - Добавить больничный

    3.  $/addDays$ - Добавить дни недели с физкультурой

    4.  $/addSpecialisation$ - Добавить специализацию

    5.  $/profile$ - Показать профиль и количество посещений

    6.  $/calculateAttendance$ - Посчитать количество посещений в неделю

    7.  $/list$ - Все ваши посещения

    8.  $/reminder$ - Включить или отключить напоминания

-   $/calculateAttendance$ - Напишите дату к которой хотите закрыться в
    виде */select* $15.12.2023$. **Ответ бота**: Чтобы закрыться к
    $15.12.2023$ вам нужно ходить: $3$ раза в неделю.

## Напоминания бота о физкультуре

Каждое воскресенье бот формирует сообщение: Привет, это Physbot. У тебя
*20* посещений, не забудь добавить посещения за прошедшую неделю. Не
забивай на физкультуру, ты всегда можешь узнать сколько раз в неделю
нужно ходить с помощью: $/calculateAttendance$. Приятных выходных!