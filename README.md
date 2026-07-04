# Media DB (RU) — Русская версия

Русская локализация плагина [obsidian-media-db-plugin](https://github.com/mProjectsCode/obsidian-media-db-plugin) с улучшенной настройкой API-источников для фильмов и игр.

## Совместимость

- Obsidian **1.12.7** и выше
- Версия плагина: **0.8.1-ru**

## Установка

1. Скопируйте папку плагина в каталог плагинов Obsidian:
   - Windows: `%APPDATA%\obsidian\plugins\obsidian-media-db-plugin\`
   - macOS: `~/Library/Application Support/obsidian/plugins/obsidian-media-db-plugin/`
   - Linux: `~/.config/obsidian/plugins/obsidian-media-db-plugin/`

2. В папке должны быть файлы: `main.js`, `manifest.json`, `styles.css`

3. Включите плагин в **Настройки → Сторонние плагины**

## Сборка из исходников

```bash
bun install
bun run build
```

После сборки `main.js` и `styles.css` появятся в корне проекта.

## Настройка API

### Фильмы

В настройках плагина раздел **«Источники данных — Фильмы»**:

| API | Сайт | Ключ |
|-----|------|------|
| **TMDB** | [themoviedb.org](https://www.themoviedb.org/settings/api) | TMDB API (Bearer Token) |
| **OMDb** | [omdbapi.com](https://www.omdbapi.com/apikey.aspx) | OMDb API Key |

### Игры

Раздел **«Источники данных — Игры»**:

| API | Сайт | Ключ |
|-----|------|------|
| **IGDB** | [dev.twitch.tv](https://dev.twitch.tv/console/apps) | Client ID + Client Secret |
| **RAWG** | [rawg.io](https://rawg.io/apidocs) | RAWG API Key |
| **Steam** | store.steampowered.com | Не требуется |
| **OMDb** | omdbapi.com | OMDb API Key |

Ключи вводятся в разделе **«API-ключи»** и хранятся в зашифрованном хранилище Obsidian.

## Использование

- **Лента** (иконка базы данных) — создать запись
- **Команды** (Ctrl+P):
  - «Создать запись» — поиск по типу медиа
  - «Создать запись (расширенный поиск)» — выбор конкретных API
  - «Создать запись по ID» — прямой поиск по ID

## Лицензия

GPL-3.0 (как оригинальный плагин)
