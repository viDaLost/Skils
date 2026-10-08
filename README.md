# Skils

Личная коллекция скилов для Claude Code. Все скилы лежат в `.claude/skills/<имя>/SKILL.md`.

## Как подключить

- **В проект:** скопировать нужные папки из `.claude/skills/` в `.claude/skills/` проекта.
- **Глобально (на своём компьютере):** скопировать их в `~/.claude/skills/`.
- **Как плагин:** `/plugin marketplace add viDaLost/Skils`, затем `/plugin install vidalost-skills@vidalost-skills`.
- **В облачной сессии Claude Code:** попросить подключить репозиторий `viDaLost/Skils`, и скилы подхватятся оттуда.

## Состав

| Скил | Источник | Для чего |
| --- | --- | --- |
| `design-taste-frontend` | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | Основной: лендинги, портфолио и редизайны без шаблонного вида (v2) |
| `design-taste-frontend-v1` | taste-skill | Старая v1 основного скила |
| `gpt-taste` | taste-skill | Более строгий вариант для GPT/Codex |
| `redesign-existing-projects` | taste-skill | Аудит и редизайн существующего UI |
| `high-end-visual-design` | taste-skill | Спокойный «дорогой» UI, мягкая анимация |
| `minimalist-ui` | taste-skill | Редакционный минимализм в стиле Notion/Linear |
| `industrial-brutalist-ui` | taste-skill | Брутализм, швейцарская типографика |
| `stitch-design-taste` | taste-skill | Правила для Google Stitch и экспорт DESIGN.md |
| `full-output-enforcement` | taste-skill | Заставляет выдавать полный код без заглушек |
| `image-to-code` | taste-skill | Сначала референсы-картинки, потом вёрстка по ним |
| `imagegen-frontend-web` | taste-skill | Генерация макетов сайтов (только изображения) |
| `imagegen-frontend-mobile` | taste-skill | Генерация макетов мобильных экранов (только изображения) |
| `brandkit` | taste-skill | Брендбук и айдентика |
| `impeccable` | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) v4.5.0 | Дизайн, аудит, критика и полировка UI: 24 команды (`/impeccable polish`, `audit`, `critique`…) |
| `design-md-library` | [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | 74 готовых DESIGN.md реальных брендов (Stripe, Linear, Apple, Vercel…) |

У каждого скила рядом лежит лицензия его источника: MIT у taste-skill и awesome-design-md, Apache 2.0 у impeccable.

`impeccable` при первом запуске скачивает свой бинарник с GitHub-релизов `pbakaus/impeccable` и проверяет его по SHA-256. Если сети нет, скил работает и без него.

## Обновление

Скилы скопированы из исходных репозиториев на дату добавления. Чтобы обновить, нужно заново скопировать папки из исходников.
