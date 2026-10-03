<div align="center">

[![Return to @Eniggman](https://img.shields.io/badge/⬅%20Return%20to-@Eniggman-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Eniggman)

# ⚡ Enigman Termux Lab 2.0

### *Autonomous Edge AI & Tooling Ecosystem on Android*

[![Termux](https://img.shields.io/badge/Termux-Android-000000?style=for-the-badge&logo=termux&logoColor=white)](https://termux.dev/)
[![FastMCP](https://img.shields.io/badge/FastMCP-2.0-blueviolet?style=for-the-badge&logo=fastapi&logoColor=white)](https://github.com/jlowin/fastmcp)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Bash](https://img.shields.io/badge/Bash-Automation-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)](https://www.gnu.org/software/bash/)
[![AI Agents](https://img.shields.io/badge/AI%20Agents-Autonomous-8E75B2?style=for-the-badge&logo=openai&logoColor=white)](https://github.com/Enigman-Termux-lab)
[![Antigravity Bionic](https://img.shields.io/badge/Antigravity-Bionic%20r29-orange?style=for-the-badge&logo=google&logoColor=white)](https://github.com/Enigman-Termux-lab/antigravity-cli-termux)
[![Lab Version](https://img.shields.io/badge/Lab%20Version-v2.0-39FF14?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Enigman-Termux-lab)
[![Release Date](https://img.shields.io/badge/Release%20Date-October%202026-007EC6?style=for-the-badge&logo=googlecalendar&logoColor=white)](https://github.com/Enigman-Termux-lab)

<br/>

**Добро пожаловать в Главный координационный зал Enigman Termux Lab!**

> **Enigman Termux** — открытая исследовательская лаборатория и экосистема инструментов, превращающая обычный Android-смартфон в автономную вычислительную ноду для локальных и облачных ИИ-агентов.  
> Здесь сходятся архитектурные чертежи, активные шлюзы и каналы удалённого управления мобильным Linux. Оставьте сложность консольных команд за порогом — ниже представлены наш манифест и полный реестр действующих модулей.

---

</div>

## 🎯 Главная цель (Миссия лаборатории)

Большинство людей используют смартфон исключительно как «экран для потребления контента». При этом внутри каждого современного устройства скрывается мощный процессор (ARM64) и 8–16 ГБ оперативной памяти — по вычислительной мощности это уровень полноценного персонального компьютера.

**Termux** превращает Android в настоящий карманный Linux без root-прав. Но у этого есть обратная сторона: **терминальная среда сложна**, требует навыков системного администрирования и крайне неудобна для набора консольных команд на маленьком сенсорном экране.

**Наша цель — превратить скрытую мощь терминала в доступный и удобный инструмент:**
Вместо того чтобы вручную воевать с чёрной консолью и синтаксисом bash, всю сложную системную работу берёт на себя **автономный ИИ-агент**. Вы управляете системой через технологии **Remote Control** — современный, интуитивный визуальный интерфейс и простое общение на человеческом языке.

1. 📱 **Карманный ПК 24/7:** Превращение смартфона в автономную рабочую станцию и микросервер (со встроенным аккумулятором-UPS и независимой связью).
2. 🎛️ **Remote Control вместо консоли:** Управление процессами терминала из удобного визуального интерфейса без необходимости печатать команды вручную.
3. 🤖 **Автономные агенты с «руками»:** Предоставление интеллекту прямого безопасного доступа к файлам и окружению для написания кода, настройки систем и выполнения задач.

---

## 🎛️ Каталог модулей лаборатории

| Инструмент / Репозиторий | Назначение и функциональность |
| :--- | :--- |
| 🛰️ **[antigravity-remote-control](https://github.com/Enigman-Termux-lab/antigravity-remote-control)** | Удалённое веб-управление Antigravity CLI в Termux (Live terminal, WebSocket, сессии) |
| ⚡ **[antigravity-cli-termux](https://github.com/Enigman-Termux-lab/antigravity-cli-termux)** | Официальный нативный порт Google Antigravity CLI под Termux (Android Bionic, NDK r29) |
| 🤖 **[codex-termux-remote-control](https://github.com/Enigman-Termux-lab/codex-termux-remote-control)** | Автономный запуск и интеграция OpenAI Codex CLI в Termux с Remote Control |
| 🎛️ **[termux-widget-shortcuts](https://github.com/Enigman-Termux-lab/termux-widget-shortcuts)** | Генератор быстрых виджетов на рабочий стол Android для запуска AI-агентов в один клик |
| 🛡️ **[opencode-termux-sandbox](https://github.com/Enigman-Termux-lab/opencode-termux-sandbox)** | Защищённая изолированная песочница PRoot (Alpine) для безопасной работы агентов |
| 🔔 **[termux-agent-notify](https://github.com/Enigman-Termux-lab/termux-agent-notify)** | Системные push-уведомления и вибрация в Android при завершении задач агентами |
| 🪝 **[termux-agent-hooks](https://github.com/Enigman-Termux-lab/termux-agent-hooks)** | Событийные хуки жизненного цикла для агентов (безопасность, перехват команд, логирование) |
| 🧹 **[termux-cleanup](https://github.com/Enigman-Termux-lab/termux-cleanup)** | Автоматическая очистка дискового пространства Termux (кеши apt, npm, pip, pnpm) |
| 🔄 **[termux-auto-updater](https://github.com/Enigman-Termux-lab/termux-auto-updater)** | Безопасное пакетное обновление CLI-инструментов с защитой от поломки путей |
| 🔌 **[termux-fix-path](https://github.com/Enigman-Termux-lab/termux-fix-path)** | Анализ архитектуры и диагностика бинарников Bionic ELF / glibc в Termux |
| 🛑 **[termux-shutdown-tools](https://github.com/Enigman-Termux-lab/termux-shutdown-tools)** | Корректное завершение фоновых демонов Termux и сохранение заряда батареи |
| 🌉 **[termux-agent-bridge](https://github.com/Enigman-Termux-lab/termux-agent-bridge)** | Универсальный MCP Gateway & Bridge для подключения внешних агентов по FastMCP / HTTP |
| 📲 **[termux-api](https://github.com/Enigman-Termux-lab/termux-api)** | Аппаратный мост к датчикам Android, буферу обмена, SMS и батарее для AI-агентов |

---

## 👤 Автор и сообщество

* Основатель и мейнтейнер: **[@Eniggman](https://github.com/Eniggman)**
* Организация на GitHub: **[Enigman-Termux-lab](https://github.com/Enigman-Termux-lab)**

Приглашаем разработчиков, энтузиастов Termux и исследователей агентных систем делиться идеями, создавать Issue и отправлять Pull Request!
