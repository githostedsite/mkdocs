#  

Установка

Описаные действия проводились для Mac OS, но должны работать и для других систем.

Есть несколько различных способов выполнения одной и той же задачи, в том числе и установить Mkdocs можно разными способами.  Я выбрал установку при помощи менеджера пакетов pip.

С [сайта Python.org] (https://python.org) скачиваем и устанавливаем актуальную версию. 

Запускаем Терминал или командную строку для Windows,  и выполняем команды:

```
pip install mkdocs mcdocs-material mkdocs-minify-plugin mkdocs-redirects
```

------



Далее я загрузил проект на Gitflic, если вы привыкли работать с другой платформой то это руководство вероятно не для вас. Информация по регистрации и авторизации на сервисе находится [здесь](https://gitflic.ru/help/profile/profile#auth)

После создания нового проекта на Gitflic мы видим инструкцию по подключению репозитория. 

 Дальнейшая инструкция для тех, кто никогда н еиспользовал аутентификацию при помощи sh-ключей. Я не утверждаю что это единственно правильный метод, а просто рассказываю как сделал это сам.

Чтобы это работало, необходимо настроить аутентификацию на сервисе. Те кто когда-либо настраивал авторизацию на GitHub без руда разберутся в процессе.
Я создал новый ssh ключ и добавил его на сайт. Пользователям Windows 7 потребуется утилита [PuTTy](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html), для более новых версий потребуется установка подсистемы Linux в настройках. 

Для linux и mac OS используем 

```
ssh-keygen
Нажимаем Enter чтобы сохранить стандартное название ключа, и вводим пароль 2 раза
```

Эта команда создала в домашней папке скрытый каталог .ssh и в нем 2 файла - id_rsa и id_rsa.pub. Открываем файл с публичным ключом и копируем единственную строку полностью, после чего выходим из редактора без сохранения:

```
nano ~/.ssh/id_rsa.pub
```

На Gitflic.ru открываем настройки в правом верхнем углу, далее **Ключи**. В поле **Публичный ключ** вставляем скопирвоанное значение, добавляем какое-нибудь название и нажимаем **Добавить**

Открываем созданный проект,

![image-20220423015226928](https://tva1.sinaimg.cn/large/e6c9d24egy1h1jayqp86xj20b105iq2z.jpg)

