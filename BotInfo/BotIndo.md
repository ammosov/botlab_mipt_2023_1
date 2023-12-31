# Jasper
## Бот для поиска людей ради различных активностей

## Краткое описание

>Jasper - бот для поиска людей по заданным тегам.

> [!NOTE]
> Эти теги могут включать как предпочтения, так и личное описание человека.


## Начало работы

Стартовый промпт бота:
```
Привет, для начала работы введи \start
```
Ответ пользователя:
```
\start - начать работу с ботом или прейти в главное меню.
```

Ответ бота:
```
1 - Начать поиск
2 - Изментить теги поиска
3 - Настройка аккаунта
4 - Теги

0 - Помощь 
```

# Выбор из главного меню
## 1 - Начать поиск

Промпт бота:
```
Поиск...
```

Описание:


Начать поиск по заданным тегам. Когда подходящий пользователь будет
найден, бот выведет информацию о нем:
``` 
Я нашел кое-кого подходященго:
{ник, возраст, язык, страна, город, если указаны}
{1-5 фотографий, если есть}
Он подходит по тегу:
{Подходящий тег}
```

И пользователю будет предоставлен выбор:


1. Пригласить - ваш профиль будет отправлен пользователю и в случае его согласия, бот
   либо отправит вам его телеграм, либо соединит вас через себя, в зависимости от настройки анонимого режима.


Промпт:
```
Приглашение отправленно. Ожитается ответ...
```


Если другой пользователь не примет или отклонит приглашение
вам будет выдано сообщение:
```
Предложенный пользователь не принял приглашение.
Поиск...
```
и ваш поиск продолжиться


2. Проигнорировать - пользователь будет добавлен в временный бан (его время настраивается в настройках), и он вам не будет предложен далее.
   Промпт:
``` 
Пользователь откланен и не будет временно вам предлагаться
Поиск...
```

## 2 - Изменить теги поиска
Промпт бота:
```
1. Выбрать одиночный тег
2. Выбрать коллекцию тегов
3. Настроить коллецию  бан-тегов
```
Бан-теги - теги, при наличии которых у другого пользователя, он не будет
предложен вам.
### 1. Выбрать одиночный тег

Промпт бота:
```
Введите тег или его id 
```

Если найден тег или его вариации:

Промпт бота:
```
1. {предложенный тег}
2. {предложенный тег}
3. {предложенный тег}
4. {предложенный тег}
5. {предложенный тег}
6. {предложенный тег}

7. Следующая страница
8. Преведущая страница
9. Назад
```

Если не найден тег или его вариации:

Промпт бота:
```
Извините, я не смог найти введеный тег или его вариации.
Измените тег или предложите его
```
### 2. Выбрать коллекцию тегов

Промпт бота:
```
1. Выбрать коллекцию
2. Настроить коллекции 
3. Создать коллекцию
```
#### 2.1. Выбрать коллекцию
Промпт бота:
```
1. {предложенная коллекция}
2. {предложенная коллекция}
3. {предложенный коллекция}
4. {предложенный коллекция}
5. {предложенный коллекция}
6. {предложенный коллекция}

7. Следующая страница
8. Преведущая страница
9. Назад
```

#### 2.2. Настроить коллекцию
Промпт бота;
```
Для начала выберите  коллекцию :

1. {предложенная коллекция}
2. {предложенная коллекция}
3. {предложенный коллекция}
4. {предложенный коллекция}
5. {предложенный коллекция}
6. {предложенный коллекция}

7. Следующая страница
8. Преведущая страница
9. Назад
```
Промпт после выбора:

``` 
Выберите действие:
1. Удалить тег
2. Добавить тег
3. Удалить коллекцию
4. Соединить с другой коллекцией
```
##### 2.2.1 Удалить тег
Будет удалять выбранные теги, пока не выбран пункт "Назад"


Промпт бота:
``` 
Выберите тег:

1. {предложенный тег}
2. {предложенный тег}
3. {предложенный тег}
4. {предложенный тег}
5. {предложенный тег}
6. {предложенный тег}

7. Следующая страница
8. Преведущая страница
9. Назад
```

##### 2.2.2 Добавить тег
Аналогично выбору одиночного тега, но будет выполняться до тех пор, пока не выбран пункт "Назад"

##### 2.2.3 Удалить коллекцию

Промпт бота:
``` 
Вы уверены, что хотите удалить коллекцию {name_collection}?
1. Да
2. Нет
```

Удаляет выбранную коллекцию или переходит в преведущее меню.

##### 2.2.3 Соединить коллекции
Промпт бота:
``` 
Выберите коллекцию для соединеия:

1. {коллекция пользователя}
2. {коллекция пользователя}
3. {коллекция пользователя}
4. {коллекция пользователя}
5. {коллекция пользователя}
6. {коллекция пользователя}

7. Следующая страница
8. Преведущая страница
9. Назад

```
Промпт бота:
``` 
Вы уверены, что хотите соеденить коллекию 
{name_collection_1} и {name_collection_2}?
1. Да
2. Нет
```
Создает новую коллекцию на основе созданных.

### 2.3 Настроить коллекцию бан-тегов
Аналогична настройки обычных коллекций тегов.

## 3 - Настройка аккаунта:
Промпт бота:
``` 
1. Настроить фото
2. Настроить свои теги
3. Анонимный режим : {Вкл.\Выкл.}
4. Временный бан
```
### 3.1 Настроить фото
Промпт бота:
``` 
1. Добавить фото
2. Удалить фото
3. Удалить все фото
```

#### 3.1.1 Добавить фото:
Промпт бота:
``` 
Отправте фото, которое хотите добавить:
```
*После отправки фото пользователем*
``` 
Введите место, на которое хотите добавить фото:
( 1 - 5 )
```

#### 3.1.2 Удалить фото:
Промпт бота:
``` 
Введите место, с которого хотите удалить фото:
( 1 - 5 )
```
#### 3.1.2 Удалить все фото:
Промпт бота:
``` 
Вы уверены, что хотите удалить все фото?
1. Да
2. Нет
```

### 3.2 Настроить свои теги
Настройка аналогична настройке одной коллекции

### 3.3 Анонимный режим
Промпт бота:
``` 
Режим анонимности изменен
```

### 3.4 Временный бан
Промпт бота:
``` 
Введите время в формате
ss/mm/hh/ddd/yy
```
В случае, если заполнены не все поля, то бот подставляет в незаполненые нули.

## 4 - Теги

Промпт бота:
``` 
1. Сайт с тегами
2. Предложить свой тег
3. Пожаловаться на тег
4. Узнать id тега
5. Топ популярных тегов
6. Топ бан-тегов
```
### 1. Сайт с тегами
Промпт бота:
``` 
{url сайта, вкладка с тегами}
```

### 2. Предложить свой тег
Промпт бота:
``` 
{url сайта, вкладка с предложениями}
```

### 3. Пожаловаться на тег
Промпт бота:
``` 
{url сайта, вкладка с жалобами}
```

### 4. Узнать id тега
Промпт бота:
``` 
{url сайта, вкладка с поиском тегов}
```

### 5. Топ популярных тегов
Пример промпта бота:

```
Топ тегов сейчас:
1. Совместная прогулка
2. Программирование
3. CS:COME
4. MineAndCraft
5. Подготовка к мат. анализу
6. Баскетбол

7. Следующая страница
8. Преведущая страница
9. Назад
```

### 6. Топ бан-тегов
Пример промпта бота:

```
Топ бан-тегов сейчас:
1. Скатываю алгосы
2. Шумерский язык
3. Doda 2
4. Политика
5. Религия
6. Гольф

7. Следующая страница
8. Преведущая страница
9. Назад
```


## Временный бан
Время, которое пользователь, которого вы не выбрали
будет не показываться вам
## Анонимный режим
Вместо отправки телеграма, бот будет соединять вас с другим пользователем через себя. При этом ваш профиль не будет отображаться ни при отправке, ни при принятии приглашений. Чтобы выйти из этого режима введите
\exit.