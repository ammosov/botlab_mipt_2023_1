# Лабораторная работа 1 курса ВШПИ

## 1 семестр 2023 года

## Краткое описание

Бот с таким функционалом является незаменимым помощником для любителей чтения. Он позволяет упростить процесс поиска и
выбора книг, а также делает процесс чтения более удобным и организованным.

1. Поиск книг - это одна из основных функций бота, которая позволяет быстро находить книги по различным параметрам,
   таким
   как название, автор, жанр и список популярных книг. Благодаря этому, пользователь может быстро найти интересующую его
   книгу и начать чтение.
2. Возможность сохранять книги в личную библиотеку позволяет пользователю всегда иметь доступ к своим любимым книгам и
   при
   необходимости возвращаться к ним. Библиотека может быть организована по жанрам, авторам или другим удобным для
   пользователя способом.
3. Функция “Цитаты” предоставляет возможность сохранять и делиться любимыми цитатами из книг. Это может быть полезно для
   поиска вдохновения, мотивации или просто для того, чтобы поделиться своими мыслями с другими.
4. Сохранение прогресса прочтения книг помогает пользователю не терять место, где он остановился, и облегчает
   возвращение к
   чтению после перерыва. Бот может отслеживать прогресс по всем книгам, которые пользователь читает в данный момент.

## Сценарии использования бота

### Формат описания:

**\*Команда***

- **\*Описание функции, которую вызывает данная команда***


- **\*Последующий диалог между ботом и пользователем***  

---

0) ***/start***

- Команда запускает бота, вызывая приветствие и выводит меню, состоящее из кнопок для управления ботом


- **Пример диалога**:  
  \- Приветствуем в библиотеке бота! 📚 Здесь вы можете искать книги по названию, автору или жанру, сохранять их в
  свою библиотеку, а также получать рекомендации на основе ваших предпочтений. Функция “Цитаты” поможет сохранить
  любимые фразы из книг, а возможность сохранять прогресс и заметки сделает чтение еще более удобным. Приятного
  пользования! 📘📙🔖


Для перехода к меню введите /menu

---

1) ***/search***

- 📖 **Поиск книг** - быстро находите книги по различным критериям: название, автор, жанр. Для каждого критерия
  применима сортировка по: популярности книги, дате выхода книги.


- **Пример диалога**:  
  \- Выберите, по какому критерию вы бы хотели найти книгу в формате:  
  \*критерий поиска* \*запрос для поиска*   
  Критерии поиска: Название, Автор, Жанр   
  Доступные жанры: Роман, Детектив, Драма, Комедия   
  \- Автор Пушкин  
  \- Страница: 1  
  \-Результаты:

1) Евгений Онегин (https://www.google.ru/books/edition/Евгений_Онегин/VSrBAQAAQBAJ?hl=ru&gbpv=1&dq=inauthor:Пушкин&printsec=frontcover)
2) История Петра I (https://www.google.ru/books/edition/История_Петра_I/f2tNEAAAQBAJ?hl=ru&gbpv=0)
3) Капитанская дочка. Живая классика (https://www.google.ru/books/edition/Капитанская_дочка_Жив/79PoDAAAQBAJ?hl=ru&gbpv=1&dq=Капитанская+дочка.+Живая+классика&printsec=frontcover)
4) Дубровский. Капитанская дочка (сборник) (https://www.google.ru/books/edition/Дубровский_Капитанск/VaAzDwAAQBAJ?hl=ru&gbpv=1&dq=Дубровский.+Капитанская+дочка&printsec=frontcover)
5) Повести Белкина. Пиковая дама (сборник) (https://www.google.ru/books/edition/Повести_Белкина_Пиков/db80DwAAQBAJ?hl=ru&gbpv=0)


Для перехода к меню введите /menu

**Критерии поиска**:  
\- **Название** - поиск по названию книги  
\- **Автор** - поиск по фамилии автора книги  
\- **Жанр** - поиск по жанру книги  
(Доступные жанры: Роман, Детектив, Драма, Комедия)

---

2) ***/my_library***

- 📚 **Моя библиотека** - сохраняйте любимые книги для того, чтобы всегда иметь возможность выбрать произведение при
  желании перечитать что-либо из списка понравившегося, а также наблюдайте за прогрессом развития собственного
  литературного познания.


- **Пример диалога**:  
  \- Выберите, что бы вы хотели сделать в библиотеке:  
  1 - Добавить книгу в библиотеку  
  2 - Получить список книг из библиотеки  
  \- 1  
  \- Введите книгу в формате \*автор книги* | \*название книги*  
  \- Пушкин | Капитанская дочка. Живая классика  
  \- Книга успешно добавлена в вашу библиотеку!


Для перехода к меню введите /menu


- **Пример диалога**:  
  \- Выберите, что бы вы хотели сделать в библиотеке:  
  1 - Добавить книгу в библиотеку  
  2 - Получить список книг из библиотеки  
  \- 2  
  \-Результаты:

1) Пушкин | Капитанская дочка. Живая классика


   Для перехода к меню введите /menu

---

3) ***/quotes***

- 💬 Цитаты - сохраняйте понравившиеся цитаты.


- **Пример диалога**:  
  \- Выберите, что бы вы хотели сделать:  
  1 - Добавить цитату  
  2 - Получить список сохранённых цитат  
  \- 1  
  \- Введите цитату в формате \*автор* | \*название книги* | \*цитата*  
  \- Пушкин | Евгений Онегин | Вдохновение — это умение приводить себя в рабочее состояние
  \- Цитата успешно добавлена!   


Для перехода к меню введите /menu


- **Пример диалога**:  
  \- Выберите, что бы вы хотели сделать:  
  1 - Добавить цитату  
  2 - Получить список сохранённых цитат  
  \- 2  
  \-Результаты:

1) Пушкин | Евгений Онегин  
   Вдохновение — это умение приводить себя в рабочее состояние


Для перехода к меню введите /menu

---

4) ***/progress***

- 🎯 **Прогресс чтения**: Следите за своим прогрессом чтения по каждой книге.


- **Пример диалога**:  
  \- Выберите, что бы вы хотели сделать:  
  1 - Изменить прогресс чтения  
  2 - Узнать прогресс чтения  
  \- 1  
  \- Введите книгу в формате \*автор* | \*название книги* | \*номер страницы, на которой вы остановились*  
  \- Пушкин | Евгений Онегин | 260
  \- Прогресс успешно сохранён!


Для перехода к меню введите /menu


- **Пример диалога**:  
  \- Выберите, что бы вы хотели сделать:  
  1 - Изменить прогресс чтения  
  2 - Узнать прогресс чтения  
  \- 2  
  \-Результаты:

1) Пушкин | Евгений Онегин | Страница 260


Для перехода к меню введите /menu