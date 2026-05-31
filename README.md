<!--
  GitHub Profile README
  Репозиторий называется так же, как ник (github.com/Tkolin/Tkolin),
  этот файл лежит в нём как README.md и становится обложкой профиля.
  Не забудь включить: Settings -> Profile -> "Include private contributions on my profile",
  чтобы граф активности показывал работу без раскрытия кода из приватных репозиториев.
-->

# Привет, я Дмитрий 👋

### Full-cycle backend-разработчик. Делаю продукт целиком, от требований до прода.

Системный анализ, архитектура, бэкенд, инфраструктура, прод. Обычно работаю один или ключевым разработчиком. Когда нужно, беру на себя и фронт, и браузерные расширения.

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

**Бэкенд:** FastAPI, Django, Laravel, REST + GraphQL + gRPC, WebSocket, gRPC streaming (Yellowstone/Geyser)
**Данные и инфра:** PostgreSQL, ClickHouse, MySQL, Redis, RabbitMQ, Elasticsearch, Docker, CI/CD, nginx, Grafana
**Фронтенд (при необходимости):** Vue 3 / Nuxt, React, Feature-Sliced Design, расширения на WXT
**AI:** интеграция GPT/LLM в продукт, разработка с Claude Code и Copilot

---

### 🛠️ Над чем работал

**Рекрутинг-платформа, владелец бэкенда и фуллстек** *(2024 - сейчас)*
Боевая система: ~5k пользователей, ~1k MAU, база на 50+ млн записей.
- Архитектура: веб-бэкенд на Django, за ним микросервисы на FastAPI (Postgres, Redis, RabbitMQ), к которым он обращается. Спроектировал и вывел в прод сервисы мониторинга изменений кандидатов.
- Аналитику складывал в ClickHouse и выводил статистику в Grafana.
- Сделал сервис истории резюме на diff-подходе: хранит разницы, а не снимки, считает на стороне SQL, поэтому занимает кратно меньше места.
- Помог реструктурировать серверную часть и сократить расходы на инфраструктуру примерно на 40%.
- Перестроил унаследованный фронт: с двух монолитных страниц на Feature-Sliced Design, с JS на TypeScript. Переписал парсер с Selenium на Playwright, расширение перевёл на WXT + Vue.

**Sleep Zero, торговая платформа на Solana (full-cycle)** *(2026)*
- Сделал продукт целиком: личный кабинет (Vue 3/Nuxt), бэкенд (FastAPI), торговое ядро и расширение.
- Торговое ядро: транзакции для 6+ лаунчпадов, real-time ончейн-данные через gRPC + Yellowstone (Geyser), WebSocket для низкой задержки.
- Покрыл бэкенд тестами: в трейдинге баг стоит реальных денег.

**СибНИПИ, система проектной документации (соло)** *(2024-2025)*
- В одиночку, от требований до рабочей системы: PHP/Laravel + GraphQL (Apollo) + React, Postgres, Docker.
- Весь жизненный цикл документации, распределение исполнителей по диаграмме Ганта и микросервис «блюпринтов» (drag-and-drop) для вычислений внутри документов.

---

### 📊 Активность

![Stats](https://github-readme-stats.vercel.app/api?username=Tkolin&show_icons=true&hide=stars&theme=default)

### 📫 Связаться

[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:p.gnedkov@tihonova.team)
