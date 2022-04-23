

Файловая структура проекта на данный момент выглядит так:

```reStructuredText
mkdocs.yml
.gitignore
README.md
robots.txt
   Docs
      - index.md
      guide
         - about-this-guide.md
         .....
         - creating-custom-theme.md
   style
      brands
      fonts
      assets
   jswebsite-theme
      - main.html
      
```

Я создал папку в корне проекта jswebsite-theme, и вместе с другими параметрами определил в mkdocs.config ее как пользовательскую папку темы:

```yaml
theme:
   name: null
   custom_dir: 'jswebsite-theme'
   locale: en
   static_templates:
      - sitemap.html
   include_sidebar: true
```

Далее я добавил минимально необходимый код в файл main.html:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>{% if page.title %}{{ page.title }} - {% endif %}{{ config.site_name }}</title>
  </head>
  <body>
    {{ page.content }}
  </body>
</html>
```



