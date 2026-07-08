# telezkaai fixed GitHub Pages package

В этой версии статья выводится прямо на главной странице `/telezkaai/`.

Что исправлено:

1. `index.md` больше не показывает пустой список постов. Он содержит саму статью.
2. `_config.yml` настроен под project page: `baseurl: "/telezkaai"`.
3. Пост в `_posts` переименован на дату в прошлом: `2024-01-01-prompt-engineering-gonzo.md`.
4. Добавлен `future: true`, чтобы Jekyll не прятал посты из-за даты/таймзоны.

Как залить:

```bash
unzip telezkaai-fixed-github-pages.zip
cd telezkaai-fixed-github-pages
cp -R . /path/to/your/local/telezkaai-repo/
cd /path/to/your/local/telezkaai-repo
git add .
git commit -m "Fix article rendering on GitHub Pages"
git push
```

После деплоя статья будет на:

https://obey177.github.io/telezkaai/

Если GitHub Pages уже включён: Settings → Pages → Deploy from a branch → main / root.
