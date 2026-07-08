# тележка эйай — GitHub Pages / Jekyll

Главная страница — `index.md`, layout `home`.
На главной автоматически показывается список постов из папки `_posts`.

## Как добавить новый пост

Создай файл в `_posts` с именем:

```text
YYYY-MM-DD-short-slug.md
```

Минимальный front matter:

```yaml
---
layout: post
title: "Название поста"
description: "Короткое описание для карточки на главной"
date: 2024-02-01 10:00:00 +0300
image: /assets/images/some-image.webp
permalink: /posts/some-post/
---
```

После пуша карточка появится на главной автоматически.

## Важно для project pages

Для адреса `https://obey177.github.io/telezkaai/` в `_config.yml` должно быть:

```yaml
baseurl: "/telezkaai"
```

Для личного сайта `https://USERNAME.github.io/` нужно поставить:

```yaml
baseurl: ""
```
