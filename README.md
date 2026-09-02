<div align="center">

# ⚡ Enigman Termux Lab

### *Autonomous Edge AI & Tooling Ecosystem on Android*

[![Termux](https://img.shields.io/badge/Termux-Android-000000?style=for-the-badge&logo=termux&logoColor=white)](https://termux.dev/)
[![FastMCP](https://img.shields.io/badge/FastMCP-2.0-blueviolet?style=for-the-badge&logo=fastapi&logoColor=white)](https://github.com/jlowin/fastmcp)
[![Python 3](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Bash](https://img.shields.io/badge/Bash-Automation-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)](https://www.gnu.org/software/bash/)
[![Google Gemini](https://img.shields.io/badge/Google-Gemini%20Pro-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://gemini.google.com/)
[![Antigravity CLI](https://img.shields.io/badge/Antigravity-CLI%20Agent-orange?style=for-the-badge&logo=google&logoColor=white)](https://github.com/Enigman-Termux-lab)

<br/>

**Enigman Termux Lab** — открытая исследовательская лаборатория и экосистема инструментов, превращающая обычный Android-смартфон в автономную вычислительную ноду для локальных и облачных ИИ-агентов.

---

</div>

## 🌐 Проекты лаборатории (Projects)

Все инструменты, скиллы публикуются в виде отдельных специализированных репозиториев прямо в этой организации:

| Проект / Инструмент | Назначение и стек | Репозиторий |
| :--- | :--- | :---: |
| ⚡ **gemini-spark-mcp-bridge** | **MCP-мост для Spark Gemini**: Управляйте Termux и Antigravity CLI(и на пк) из веб-интерфейса Google Gemini Spark по FastMCP / Streamable HTTP. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/gemini-spark-mcp-bridge) |

> 💡 Полный список текущих и будущих разработок доступен во вкладке **[Repositories](https://github.com/orgs/Enigman-Termux-lab/repositories)**.

---

## ❓ Что такое Termux простыми словами?

Большинство людей используют смартфон только как «экран для соцсетей». При этом внутри современного телефона установлен мощный процессор (ARM64) и 8–16 ГБ оперативной памяти — по мощности это сопоставимо с хорошим офисным ноутбуком.

> **Termux** — это полноценный **карманный Linux** внутри твоего Android-смартфона, которому **НЕ нужны root-права**.

Это не просто чёрное окно с мигающим курсором. После установки ты получаешь настоящую операционную систему:
* 📦 **Любые инструменты разработчика:** внутри есть собственный пакетный менеджер (`pkg install`), где одной командой ставятся `Python`, `Node.js`, `Git`, `OpenSSH`, базы данных и компиляторы.
* 🔋 **Автономный микросервер 24/7:** телефон мало потребляет, у него есть встроенный аккумулятор (UPS), мобильный интернет и Wi-Fi. Он может сутками работать в кармане или на тумбочке как сервер автоматизации.
* 📲 **Доступ к железу смартфона (через Termux:API):** скрипты могут читать уровень заряда батареи, управлять Wi-Fi, отправлять системные уведомления, делать снимки с камеры и работать с датчиками.
* 🔘 **Запуск в один тап (через Termux:Widget):** сложные цепочки команд и серверов можно повесить на обычные кнопки-виджеты на рабочем столе Android.

---

## 🎯 Зачем всё это и моя цель (Миссия лаборатории)

Обычно умные облачные нейросети (Google Gemini, ChatGPT, Claude) заперты в веб-браузере: они могут только отвечать текстом, но у них «нет рук», чтобы реально что-то сделать на твоём устройстве или компьютере.

**Моя цель — превратить связку Android + Termux в:**
1. 📱 **Edge AI Node**: Полноценный микросервер, доступный 24/7 для выполнения фоновых задач, сбора телеметрии и хостинга локальных агентов.
2. 🔌 **Universal MCP Hub**: Стандартизированный узел, предоставляющий облачным ИИ-моделям (Gemini Spark, Claude, GPT) безопасный доступ к файловой системе, терминалу, системным утилитам и датчикам Android.
3. 🦾 **Autonomous Pair-Programming**: Возможность ставить задачи ИИ-агентам прямо с телефона и контролировать их выполнение через виджеты в один клик.

---

## 🏗️ Архитектура экосистемы

```text
  ┌──────────────────────────────────────────────────────────────┐
  │                 Облачные LLM / Веб-интерфейсы                │
  │        (Gemini Spark, Google AI Studio, Claude, GPT)         │
  └──────────────────────────────┬───────────────────────────────┘
                                 │
                                 │ Model Context Protocol (Streamable HTTP / SSE)
                                 ▼
  ┌──────────────────────────────────────────────────────────────┐
  │                   Android Phone (Termux)                     │
  │                                                              │
  │   ┌────────────────────────┐      ┌───────────────────────┐  │
  │   │      MCP Bridges       │ ◄──► │     AI Agent Skills   │  │
  │   │  (Uvicorn + FastMCP)   │      │  (System Prompts, SOP)│  │
  │   └───────────┬────────────┘      └───────────────────────┘  │
  │               │                                              │
  │               ▼                                              │
  │   ┌────────────────────────┐      ┌───────────────────────┐  │
  │   │   Termux Core Engine   │ ◄──► │   Termux:Widget &     │  │
  │   │ (Bash, Python, Git, gh)│      │   Hardware Sensors    │  │
  │   └───────────┬────────────┘      └───────────────────────┘  │
  │               │                                              │
  │               ▼                                              │
  │   ┌────────────────────────┐                                 │
  │   │    Antigravity CLI     │ (Автономный AI кодинг-агент)    │
  │   └────────────────────────┘                                 │
  └──────────────────────────────────────────────────────────────┘
```
---

## 👤 Автор и сообщество

* Основатель и мейнтейнер: **[@Eniggman](https://github.com/Eniggman)**
* Организация на GitHub: **[Enigman-Termux-lab](https://github.com/Enigman-Termux-lab)**

Приглашаем разработчиков, энтузиастов Termux и исследователей агентных систем делиться идеями, создавать Issue и отправлять Pull Request!

---

#termux #android #mcp #fastmcp #gemini-spark #antigravity #ai-agents #streamable-http #edge-ai #linux-on-android
