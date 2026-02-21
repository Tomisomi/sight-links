# sight-links

Статическая Linktree-страница с готовой конфигурацией для Cloudflare.

## Локальный запуск

```bash
python3 -m http.server 4173 --bind 0.0.0.0
```

## Деплой в Cloudflare Pages (через Git)

В настройках проекта Cloudflare Pages укажи:

- **Build command**: *(пусто)*
- **Build output directory**: `.`

## Деплой в Cloudflare Workers (через Wrangler)

В репозитории уже добавлен `wrangler.toml` c `assets`-конфигурацией, поэтому можно деплоить как статический сайт:

```bash
npx wrangler deploy
```

Wrangler поднимет `index.html` из корня проекта как статический ассет.
