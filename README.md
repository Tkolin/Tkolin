<!--
  GitHub Profile README
  Репозиторий называется так же, как ник (github.com/Tkolin/Tkolin),
  этот файл лежит в нём как README.md и становится обложкой профиля.
  Не забудь включить: Settings -> Profile -> "Include private contributions on my profile",
  чтобы граф активности показывал работу без раскрытия кода из приватных репозиториев.
-->

# Привет, я Дмитрий 👋

### Full-cycle backend-разработчик. Делаю продукт целиком, от требований до прода.

Системный анализ, UX, архитектура, бэкенд, инфраструктура, прод. Часто начинаю один и дальше веду разработку как ключевой разработчик. Когда нужно, беру на себя и фронт, и браузерные расширения.

Большая часть кода - в приватных репозиториях компаний и клиентов, так что этот профиль скорее карта того, *что* и *как* я строил, а не выкладка кода. Про архитектуру и решения с радостью расскажу на созвоне.

---

### 🧰 Стек

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
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

**Языки:** Python, SQL, TypeScript / JavaScript, PHP, C#
**Бэкенд:** FastAPI, Django, Celery / Celery Beat, Laravel, REST, GraphQL (Apollo), gRPC (Protobuf), WebSocket, gRPC streaming (Yellowstone/Geyser), ORM (SQLAlchemy, Django ORM, Eloquent), миграции схемы БД, идемпотентность, вебхуки, rate limiting, валидация данных, документация API (Swagger/OpenAPI, GraphQL playground), Telegram-боты
**Данные:** PostgreSQL, ClickHouse, MySQL, MS SQL, Redis, Elasticsearch, RabbitMQ, шифрование данных, проектирование и оптимизация БД, индексы, курсорная пагинация, EXPLAIN ANALYZE
**Инфра / DevOps:** Docker, Docker Compose, Docker Swarm (оркестрация, overlay/VIP-сети, routing mesh, реплики, rolling-update, configs/secrets), CI/CD (GitHub Actions), AWS, Yandex Cloud, S3, nginx, DNS, Cloudflare CDN, HTTP/2, SSL / Let's Encrypt, бэкапы, firewall, systemd, health/readiness-проверки, развёртывание VPS, мониторинг и алертинг (Grafana)
**Тестирование / QA:** pytest с моками, юнит- и интеграционные тесты, e2e и автоматизация браузера (Playwright, Selenium)
**Авторизация:** JWT, OAuth, вход через Telegram
**AI / LLM:** интеграция LLM в продукт, универсальный сервис под несколько провайдеров (OpenAI, DeepSeek, Gemini), локальные модели через Ollama, разработка с Claude Code и Copilot
**Блокчейн:** Solana (solana-py, solders), торговые транзакции, 6+ лаунчпадов, real-time ончейн-данные (gRPC streaming), priority fees / MEV-защита / симуляция через релей, управление кошельками и шифрование ключей, мультиплексирование RPC, PnL-трекинг
**Фронтенд:** Vue 3, Nuxt (SSR/SSG, SEO), React, Ant Design, Vuetify, SCSS, собственный UI-kit, Feature-Sliced Design, i18n, сборка (Vite, Webpack)
**Браузерные расширения:** WXT + Vue, чистый HTML/JS, Manifest V3, content scripts, background / service worker, messaging, инъекция в DOM сторонних страниц, публикация в Chrome Web Store
**Проектирование:** UX-проектирование, прототипирование, системный анализ, UML (use-case, sequence)
**Процессы / команда:** написание ТЗ, code review, git-flow, координация тестировщиков, внедрение линтеров и типизации
**Прочее:** парсинг, генерация и экспорт документов (LibreOffice), почта (POP3, IMAP), линтеры (Ruff, ESLint)

---

### 🛠️ Над чем работал

**Рекрутинг-платформа, владелец бэкенда и фуллстек** *(2023 - сейчас)*
Боевая система: ~5k пользователей, ~1k MAU, база на 50+ млн записей.
- Архитектура: веб-бэкенд на Django + Celery, за ним микросервисы на FastAPI (Postgres, Redis, RabbitMQ). Django общается с ними по REST и через очереди RabbitMQ. Спроектировал и вывел в прод сервисы мониторинга изменений кандидатов по расписанию на Celery Beat.
- Аналитику складывал в ClickHouse, статистику выводил в Grafana, файлы хранил в S3. Платежи на ЮKassa с вебхуками и идемпотентностью.
- Сделал сервис истории резюме на diff-подходе: хранит разницы, а не снимки, считает на стороне SQL, поэтому занимает порядка 10% от объёма основной базы.
- Ускорил отдачу страниц с ~20 с до ~6 с: оптимизировал работу с базой на 50+ млн записей (анализ планов через EXPLAIN ANALYZE, индексы, курсорная пагинация) и добавил кеш на тяжёлые ручки.
- Прикрутил LLM в продукт: универсальный сервис под несколько провайдеров (OpenAI, DeepSeek, Gemini), локальные модели через Ollama для удешевления.
- DevOps: VPS с нуля (firewall, systemd, SSL), CI/CD на GitHub Actions, Docker Compose, Cloudflare CDN. Помог реструктурировать серверную часть и сократить расходы на инфраструктуру примерно на 40%.
- Поднял оркестрацию на Docker Swarm: два кластера по два узла, 32 сервиса под управлением. Изолированные VIP-сети поверх overlay с service discovery и балансировкой через routing mesh, реплики ключевых сервисов с авто-перезапуском, rolling-обновления и rollback без простоя, секреты в Docker secrets.
- Перестроил унаследованный фронт: с двух монолитных страниц на Feature-Sliced Design, с JS на TypeScript. Переписал парсер с Selenium на Playwright: автоматизировал вход в аккаунты (экономило до часа в день), сессии между запусками, headless, скорость с ~2 с на запрос до ~3 rps. Расширение перевёл на WXT + Vue (Manifest V3, инъекция в DOM сайтов, опубликовано в Chrome Web Store).
- Генерация документов и экспорт через LibreOffice.

**SlipZero, торговая платформа на Solana (full-cycle)** *(2026)*
- Сделал продукт целиком: личный кабинет (Vue 3/Nuxt), бэкенд (Django + Celery и FastAPI), торговое ядро, криптоплатежи, два Telegram-бота и расширение.
- Торговое ядро: транзакции для 6+ лаунчпадов (solana-py, solders) через релей (~600 мс, priority fees, MEV-защита, симуляция), real-time ончейн-данные через gRPC + Yellowstone (Geyser) с пушем за ~200 мс. PnL-трекинг и шифрование ключей кошельков написал сам.
- Развернул торговый бэкенд на 4 серверах в разных регионах: каждый пользователь идёт через ближайший, пуш по WebSocket доходит за ~200 мс.
- Покрыл бэкенд тестами на ~80% (pytest с моками): в трейдинге баг стоит реальных денег.

**СибНИПИ, система проектной документации (ведущий разработчик)** *(2022 - 2023)*
- В одиночку, от требований до рабочей системы: PHP/Laravel + GraphQL (Apollo) + React, Postgres, Docker.
- Весь жизненный цикл документации, распределение исполнителей по диаграмме Ганта (ECharts) и микросервис «блюпринтов» - нодовый редактор как в серьёзных движках, тянешь блоки с математикой мышкой и собираешь расчёт прямо для документов, генерация через LibreOffice.

---

### 📊 Активность

![Stats](https://github-readme-stats.vercel.app/api?username=Tkolin&show_icons=true&hide=stars&theme=default)

### 📫 Связаться

[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Tk0lin)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:tkolinwork@gmail.com)
