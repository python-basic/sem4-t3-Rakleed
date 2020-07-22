# Содержание
- [ИСР № 3](#инвариативная-самостоятельная-работа--3)
    - [1 задание](#31-разработка-классов-и-объектов-запись-комментарий-для-приложения-блог-использование-наследования)
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

    def show_comment(self, comment=object):
        print(f'Никнейм: "{comment.nickname}", текст комментария: "{comment.comment_text}".')


class Comment(Post):
    def __init__(self, nickname, comment_text):
        self.nickname = nickname
        self.comment_text = comment_text


post_test = Post("Иван Александров", "Какая-то интересная статья.")
comment_test = Comment("var_inb2", "Great job!")
post_test.show_comment(comment=comment_test)
```
![Result of indepworkinvar3-1](src/programming4-indepworkinvar3-1-result.png)

### [3.2. Создание геттеров и сеттеров для классов «запись», «комментарий» приложения «Гостевая книга», а также функций для вывода на печать информации, хранящийся в объектах.](https://repl.it/@Rakleed/programming4-indepworkinvar3-2)
```python
"""
    Автор: Моисеенко Павел, группа № 1, подгруппа № 2.

    ИСР 3.2. Задание: создать геттеры и сеттеры для классов «запись»,
    «комментарий» приложения «Гостевая книга», а также функции для
    вывода на печать информации, хранящийся в объектах.

"""


class Post:
    def __init__(self, author, post_text):
        self.__author = author
        self.__post_text = post_text

    def show_comment(self, comment=object):
        print(f'Никнейм: "{comment.nickname}", текст комментария: "{comment.comment_text}".')


class Comment(Post):
    def __init__(self, nickname, comment_text):
        self.__nickname = nickname
        self.__comment_text = comment_text

    @property
    def nickname(self):
        return self.__nickname

    @nickname.setter
    def title(self, value):
        self.__nickname = str(value)

    @nickname.deleter
    def title(self):
        self.__nickname = None

    @property
    def comment_text(self):
        return self.__comment_text

    @comment_text.setter
    def comment_text(self, value):
        self.__comment_text = str(value)

    @comment_text.deleter
    def comment_text(self):
        self.__comment_text = None

    def show(self):
        print("Автор: " + str(self.author))
        print("Текст поста: " + str(self.post_text))


post_test = Post("Пётр Михайлов", "Какая-то классная статья.")
comment_test = Comment("alex_356", "Nice!")
post_test.show_comment(comment=comment_test)
```
![Result of indepworkinvar3-2](src/programming4-indepworkinvar3-2-result.png)

# [Вариативная самостоятельная работа № 3](https://repl.it/@Rakleed/programming4-indepworkvar3)
```python

```
![Result of indepworkvar3](src/programming4-indepworkvar3-result.png)
