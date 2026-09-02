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
| ⚡ **gemini-spark-mcp-bridge** | **Флагманский двусторонний MCP-мост**: удалённое управление Termux и Antigravity CLI из веб-интерфейса Google Gemini Spark по FastMCP / Streamable HTTP. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/gemini-spark-mcp-bridge) |

> 💡 Полный список текущих и будущих разработок доступен во вкладке **[Repositories](https://github.com/orgs/Enigman-Termux-lab/repositories)**.

---

## 🎯 Миссия лаборатории

Современные смартфоны обладают внушительной вычислительной мощностью (ARM64, 8-16 GB RAM, NPU), но большую часть времени простаивают в кармане.

Наша цель — превратить связку **Android + Termux** в:
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

## 🧩 Ключевые технологические столпы

* **Protocol-First (MCP):** Вся интеграция строится вокруг открытого стандарта Model Context Protocol от Anthropic и Google.
* **Security by Design:** Двусторонние туннели с защищёнными путями, разделение привилегий и адаптация под политики безопасности моделей.
* **One-Tap UX:** Никакого ручного ввода длинных команд на экранной клавиатуре — все ключевые сценарии вынесены в виджеты на рабочий стол смартфона.

---

## 👤 Автор и сообщество

* Основатель и мейнтейнер: **[@Eniggman](https://github.com/Eniggman)**
* Организация на GitHub: **[Enigman-Termux-lab](https://github.com/Enigman-Termux-lab)**

Приглашаем разработчиков, энтузиастов Termux и исследователей агентных систем делиться идеями, создавать Issue и отправлять Pull Request!
