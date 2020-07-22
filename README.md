# Содержание
- [ИСР № 3](#инвариативная-самостоятельная-работа--3)
    - [1 задание]
    - [2 задание]
- [ВСР № 3](#вариативная-самостоятельная-работа--3)

# Инвариативная самостоятельная работа № 3
### [3.1. Разработка классов и объектов «запись», «комментарий» для приложения «Блог» (использование наследования).](https://repl.it/@Rakleed/programming4-indepworkinvar3-1)
```python
"""
    Автор: Моисеенко Павел, группа № 1, подгруппа № 2.

    ИСР 3.1. Задание: разработать классы и объекты «запись»,
    «комментарий» для приложения «Блог» (использую наследование).

"""


class Post:
    def __init__(self, author, post_text):
        self.__author = author
        self.__post_text = post_text


class Comment(Post):
    def __init__(self, nickname, comment_text):
        self.__nickname = nickname
        self.__comment_text = comment_text
```

### [3.2. ](https://repl.it/@Rakleed/programming4-indepworkinvar3-2)
```python

```
![Result of indepworkinvar3-2](src/programming4-indepworkinvar3-2-result.png)

# [Вариативная самостоятельная работа № 3](https://repl.it/@Rakleed/programming4-indepworkvar3)
```python

```
![Result of indepworkvar3](src/programming4-indepworkvar3-result.png)
