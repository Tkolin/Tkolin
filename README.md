<!--
  GitHub Profile README
  Репозиторий называется так же, как ник (github.com/Tkolin/Tkolin),
  этот файл лежит в нём как README.md и становится обложкой профиля.
  Не забудь включить: Settings -> Profile -> "Include private contributions on my profile",
  чтобы граф активности показывал работу без раскрытия кода из приватных репозиториев.
-->

# Привет, я Дмитрий 👋

### Full-cycle backend-инженер. Один закрываю то, на что обычно нужна команда.

Системный анализ, UX, архитектура, бэкенд, инфраструктура, прод. Часто начинаю один и дальше веду разработку как ключевой разработчик. При необходимости беру на себя и фронтенд, и браузерные расширения.

Большая часть кода в **приватных репозиториях компаний и клиентов**, поэтому этот профиль скорее карта того, *что* я строил и *как*, а не свалка кода. С радостью разберу архитектуру и решения на созвоне.

---

### 🧰 Стек

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat&logo=elasticsearch&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244c5a?style=flat&logo=google&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat&logo=graphql&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vuedotjs&logoColor=white)
![Solana](https://img.shields.io/badge/Solana-9945FF?style=flat&logo=solana&logoColor=white)

**Бэкенд:** FastAPI, Django, Celery / Celery Beat, Laravel, REST + GraphQL + gRPC (Protobuf), WebSocket, gRPC streaming (Yellowstone/Geyser), ORM (SQLAlchemy, Django ORM, Eloquent), вебхуки, идемпотентность, Telegram-боты
**Данные и инфра:** PostgreSQL, MySQL, Redis, RabbitMQ, Elasticsearch, Docker / Docker Compose, CI/CD (GitHub Actions), nginx, Cloudflare CDN
**Блокчейн:** Solana (solana-py, solders), транзакции через релей (priority fees, MEV, симуляция), мультиплексирование RPC, PnL-трекинг
**Фронтенд (при необходимости):** Vue 3 / Nuxt (SSR/SSG), React, Feature-Sliced Design, расширения на WXT (Manifest V3, инъекция в DOM, Chrome Web Store)
**AI:** интеграция LLM в продукт, универсальный сервис под несколько провайдеров (OpenAI, DeepSeek, Gemini), локальные модели через Ollama, разрабатываю с Claude Code и Copilot

---

### 🛠️ Избранные проекты

**Рекрутинг-платформа, владелец бэкенда и фуллстек** *(2023 - сейчас)*
Боевая система: ~5k пользователей, ~1k MAU, база на **50+ млн записей**.
- Спроектировал и вывел в прод микросервисы с нуля (FastAPI, Postgres, Redis, RabbitMQ) для мониторинга изменений кандидатов по расписанию на Celery Beat.
- Сервис **истории резюме на diff-подходе**: хранит разницы, а не снимки, вычисления на стороне SQL, поэтому занимает порядка 10% от объёма основной базы.
- Ускорил отдачу страниц с ~20 с до ~6 с: оптимизировал работу с базой на 50+ млн записей (EXPLAIN ANALYZE, индексы, курсорная пагинация) и добавил кеш на тяжёлые ручки. Платежи ЮKassa с вебхуками и идемпотентностью.
- Прикрутил LLM в продукт: универсальный сервис под несколько провайдеров (OpenAI, DeepSeek, Gemini), локальные модели через Ollama для удешевления.
- DevOps: VPS с нуля (firewall, systemd, SSL), CI/CD на GitHub Actions, Docker Compose, Cloudflare CDN. Помог реструктурировать серверную часть и **сократить расходы на инфраструктуру на ~40%**.
- Перестроил унаследованный фронт: 2 монолитные страницы перевёл на Feature-Sliced Design, JS на TypeScript; переписал парсер с Selenium на Playwright (автологин экономил до часа в день, сессии между запусками, headless, с ~2 с на запрос до ~3 rps); расширение перевёл на WXT + Vue (Manifest V3, инъекция в DOM сайтов, Chrome Web Store). Генерация документов и экспорт через LibreOffice.

**SlipZero, торговая платформа на Solana (full-cycle)** *(2026)*
- Сделал продукт целиком: личный кабинет (Vue 3/Nuxt), бэкенд (Django + Celery и FastAPI), торговое ядро, криптоплатежи, два Telegram-бота и расширение.
- Торговое ядро: построение транзакций для **6+ лаунчпадов** (solana-py, solders) через релей (~600 мс, priority fees, MEV-защита, симуляция), real-time стриминг ончейн-данных через **gRPC + Yellowstone (Geyser)** с пушем за ~200 мс. PnL-трекинг и шифрование ключей кошельков написал сам.
- **Покрытие бэкенда тестами ~80% (pytest с моками)**: в трейдинге ошибка означает потерю денег.

**СибНИПИ, система проектной документации (ведущий разработчик)** *(2022 - 2023)*
- В одиночку, от требований до рабочей системы: PHP/Laravel + GraphQL (Apollo) + React, Postgres, Docker.
- Полный жизненный цикл документации, распределение исполнителей по диаграмме Ганта (ECharts) и микросервис «блюпринтов»: нодовый редактор как в серьёзных движках, тянешь блоки с математикой и собираешь расчёт прямо для документов, генерация через LibreOffice.

---

### 📫 Связаться

[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Tk0lin)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:tkolinwork@gmail.com)
