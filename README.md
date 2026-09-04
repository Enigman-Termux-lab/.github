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

## 🌐 Проекты лаборатории

Все инструменты, скиллы публикуются в виде отдельных специализированных репозиториев прямо в этой организации:

| Проект / Инструмент | Назначение и стек | Репозиторий |
| :--- | :--- | :---: |
| ⚡ **gemini-spark-mcp-bridge** | **MCP-мост для Spark Gemini**: Управляйте Termux и Antigravity CLI (и на ПК) из веб-интерфейса Google Gemini Spark по FastMCP / Streamable HTTP. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/gemini-spark-mcp-bridge) |
| 🤖 **codex-termux-remote-control** | **Codex Remote Control**: Подключение OpenAI Codex CLI в Termux к мобильному приложению ChatGPT Remote Control + виджеты быстрого запуска. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/codex-termux-remote-control) |
| 🔘 **termux-widget-shortcuts** | **Виджеты и ярлыки**: Готовые шаблоны и руководство по созданию виджетов рабочего стола Termux:Widget и Android Dynamic Shortcuts. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-widget-shortcuts) |
| 🔧 **termux-fix-path** | **Termux Fix Path**: Диагностика и исправление ошибок запуска Linux CLI-утилит (shebang, Bionic ELF, glibc, библиотека linker). | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-fix-path) |
| 🛡️ **opencode-termux-sandbox** | **OpenCode Sandbox**: Изолированная контейнерная песочница на базе Alpine Linux (PRoot-Distro) для безопасной работы AI-агентов. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/opencode-termux-sandbox) |
| 🔔 **termux-agent-notify** | **Agent Notify**: Android Push-уведомления и тактильный виброотклик по готовности ответов фоновых AI-агентов (Antigravity, OpenCode). | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-agent-notify) |
| ⚡ **termux-shutdown-tools** | **Shutdown & Wakelock**: Чистый экзит фоновых процессов, предотвращение скрытого разряда батареи и управление CPU Wakelock. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-shutdown-tools) |
| 🧹 **termux-cleanup** | **Безопасная очистка**: Удаление устаревших кэшей apt, npm, pip, pnpm store, логов и временных файлов без риска поломки окружения. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-cleanup) |
| 🔄 **termux-auto-updater** | **Безопасное автообновление**: Автоматизированное обновление пакетов и CLI-агентов с защитой shebang и путей по стандарту termux-fix-path. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-auto-updater) |
| 📱 **termux-api** | **Hardware & Sensor Bridge**: Набор скриптов и скилл прямого доступа автономных AI-агентов к аппаратным сенсорам, батарее и Android API. | [Перейти к проекту](https://github.com/Enigman-Termux-lab/termux-api) |

> 💡 Полный список текущих и будущих разработок доступен во вкладке **[Repositories](https://github.com/orgs/Enigman-Termux-lab/repositories)**.

---

## 🎯 Что такое Termux и моя цель (Миссия лаборатории)

Большинство людей используют смартфон только как «экран для соцсетей». При этом внутри современного телефона установлен мощный процессор (ARM64) и 8–16 ГБ оперативной памяти — по вычислительной мощности это уровень полноценного ноутбука.

> **Termux** превращает Android в настоящий **карманный Linux без root-прав**, где одной командой (`pkg install`) ставятся `Python`, `Node.js`, `Git`, `OpenSSH`, базы данных, а через `Termux:API` есть прямой доступ к датчикам, батарее и системным функциям смартфона.

С другой стороны — современные облачные нейросети (Google Gemini, Claude, ChatGPT), которые заперты в веб-браузерах: они отлично рассуждают и пишут код, но у них **нет «рук»**, чтобы запустить скрипт или протестировать решение на реальном железе.

**Моя цель — объединить интеллект ИИ и возможности Termux через открытый протокол MCP:**
1. 📱 **Edge AI Node**: Смартфон становится автономным микросервером 24/7 (со своим аккумулятором-UPS и мобильной связью) для фоновых задач и локальных вычислений.
2. 🔌 **Universal MCP Hub**: Безопасный мост, дающий облачным моделям (Gemini Spark и др.) прямой доступ к терминалу, файлам и датчикам Android или рабочего ПК.
3. 🦾 **One-Tap AI Automation**: Запуск кодинг-агента (**Antigravity CLI**) и сложных цепочек автоматизации в один клик прямо с виджетов на рабочем столе смартфона.

---

## 👤 Автор и сообщество

* Основатель и мейнтейнер: **[@Eniggman](https://github.com/Eniggman)**
* Организация на GitHub: **[Enigman-Termux-lab](https://github.com/Enigman-Termux-lab)**

Приглашаем разработчиков, энтузиастов Termux и исследователей агентных систем делиться идеями, создавать Issue и отправлять Pull Request!

---

#termux #android #mcp #fastmcp #gemini-spark #antigravity #ai-agents #streamable-http #edge-ai #linux-on-android
