

Настроим основные параметры сайта, открыв файл mkdocs.yml в редакторе который вы выбрали. Я использую VS code для html, css, скриптов и конфигурационных файлов из-за привычки. Если вы не работали с ним ранее, то для Windows я бы посоветовал notepad++, это блокнот с подсветкой синтаксиса, нумерация строк и возможность открыть несколько файлов во вкладках одного окна.

Определим основные параметры и подключим к сайту тему оформления Material, для отредактируем конфигурационный файл следующим образом:

```yaml
# Настройки проекта
site_name: githosted.ru    
site_url: https://githosted.ru
site_author: Vasilii Pavlov
site_description: Create site to host documentation 

# настройки репозитория
repo_name: githostedsite
repo_url: https://gitflic.ru/projects/githostedsite/githostedsite
edit_url: ""

# Авторские права
copyright: 2022 https://githosted.ru

# Параметры темы:
theme: 
   name: material
```

Видим в браузере, что изменился дизайн сайта, появилась ссылка на репозиторий, навигация, копирайт и поиск по сайту. 

Определим в конфигурации дополнительные параметры. 









