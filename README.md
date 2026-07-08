# Prompt Engineering Gonzo — Jekyll / GitHub Pages

Готовый мини-сайт под GitHub Pages.

## Что внутри

- `_posts/2026-07-08-prompt-engineering-gonzo.md` — статья с Jekyll front matter.
- `assets/images/` — картинки в PNG и WebP.
- `_layouts/` — минимальные HTML-шаблоны.
- `assets/css/style.css` — тёмный стиль страницы.
- `_config.yml` — настройки Jekyll.
- `Gemfile` — для локального запуска через github-pages gem.

## Быстрый деплой через GitHub UI

1. Создай новый репозиторий на GitHub.
   - Для личного сайта: `USERNAME.github.io`.
   - Для проектного сайта: любое имя, например `ai-notes`.
2. Загрузи содержимое этой папки в репозиторий.
3. Открой `Settings → Pages`.
4. В `Build and deployment` выбери `Deploy from a branch`.
5. Branch: `main`, folder: `/root`.
6. Сохрани. Через пару минут сайт появится по адресу:
   - `https://USERNAME.github.io/` для личного сайта;
   - `https://USERNAME.github.io/REPOSITORY/` для проектного сайта.

## Деплой через терминал

```bash
git init
git add .
git commit -m "Add prompt engineering post"
git branch -M main
git remote add origin git@github.com:USERNAME/REPOSITORY.git
git push -u origin main
```

Потом включи GitHub Pages в настройках репозитория: `Settings → Pages → Deploy from a branch → main / root`.

## Локальный запуск

```bash
bundle install
bundle exec jekyll serve
```

Открой `http://localhost:4000`.

Если это проектный сайт, а не `USERNAME.github.io`, можно прописать имя репозитория в `_config.yml`:

```yml
baseurl: "/REPOSITORY"
```
