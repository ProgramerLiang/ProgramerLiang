# ProgramerLiang · 科瑞颇

学生。写东西从「自己用得着」出发：agent 工具链、Linux 桌面自动化，以及一些折腾出来的小程序。
做完再开源，顺手把边界和坑写清楚。

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/ProgramerLiang?tab=repositories&language=python)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://github.com/ProgramerLiang?tab=repositories&language=javascript)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://github.com/ProgramerLiang?tab=repositories&language=typescript)
[![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)](https://github.com/ProgramerLiang?tab=repositories&language=kotlin)
[![Linux](https://img.shields.io/badge/Linux-Wayland%20%2F%20X11-FCC624?style=flat-square&logo=linux&logoColor=black)](https://github.com/ProgramerLiang/pi-computer-use)

---

## 现在在做什么

两个 PI-Desktop 插件：一个把 Linux 桌面交给 agent 操作，一个让主 agent 只做编排、把活派给独立会话。

### [PI Computer Use](https://github.com/ProgramerLiang/pi-computer-use) · [插件中心](https://plugins.aiuo.net/plugins/corripo.computer-use)

Linux 桌面的 computer use 插件：截屏（整屏或区域）、鼠标移动 / 点击 / 滚动、文本与组合键输入，外加会话探测和窗口枚举。
Wayland 走 `grim` + `ydotool`（纯打字可用 `wtype`），X11 走 `import` / `scrot` + `xdotool`；依赖按能力安装，不需要两套后端同时存在。
Wayland 下 fcitx5 文本注入默认 fail-closed，需显式允许短暂停用输入法。

插件 id `corripo.computer-use` · v0.1.2 · JavaScript

### [Superagent Orchestrator](https://github.com/ProgramerLiang/piD-super-agent) · [插件中心](https://plugins.aiuo.net/plugins/corripo.superagent-orchestrator)

让主 agent 把任务派给独立的 worker 会话，派完就结束本轮，结果自己回来。
给模型一个 `SessionTask` 工具（`spawn` / `spawnIn` / `send` / `supervise` / `status` / `result` / `wait` / `accept` 等 12 个 action）、一个 Workers 视图，以及 `state` / `human_action` 状态契约 —— 让「做完了」和「要你决定」在卡片上分得开。

插件 id `corripo.superagent-orchestrator` · v0.1.1 · MIT · JavaScript

---

## 精选项目

| 项目 | 说明 | 主要语言 |
| :--- | :--- | :--- |
| [ESHTTC-Senior-IT](https://github.com/ProgramerLiang/ESHTTC-Senior-IT) | 教师进修学校附属实验学校高中信息课 | Python |
| [salt-player-for-linux](https://github.com/ProgramerLiang/salt-player-for-linux) | Salt Player（椒盐音乐）的 Linux 桌面版，基于 SaltUI + Compose Multiplatform：本地扫描、内嵌封面、四种播放模式、配置持久化 | Kotlin |
| [oh-my-omp](https://github.com/ProgramerLiang/oh-my-omp) | [oh-my-pi](https://github.com/can1357/oh-my-pi) 的终端配置面板，用 omp 自己的 TUI 框架做成标签页式交互界面 | TypeScript |
| [SinWaveGame](https://github.com/ProgramerLiang/SinWaveGame) | 正弦型函数小游戏，用方向键调振幅 A、角频率 ω、初相 φ 观察波形变化 | Python |
| [hangman-for-mb9p](https://github.com/ProgramerLiang/hangman-for-mb9p) | 小米手环 9 Pro 上的 HANGMAN 猜单词小游戏（Vela JS），含连胜计分与按键振动反馈 | JavaScript |

---

## 环境与工具

- **语言** — Python · JavaScript · TypeScript · Kotlin
- **运行时与框架** — Node.js · Compose Multiplatform · Vela JS
- **平台** — Linux（Wayland / X11）
- **工程** — Git · GitHub Actions（见 `salt-player-for-linux` 的 CI）

<sub>想查具体依赖和构建方式？每个仓库的 README 里都写了版本要求和缺依赖时的报错行为。</sub>

---

## 数据

<sub>下面的统计卡由第三方服务 [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) 实时生成，需要联网加载，可能较慢或偶发失败。</sub>

<img height="150" alt="GitHub 统计" src="https://github-readme-stats.vercel.app/api?username=ProgramerLiang&show_icons=true&hide_title=true&hide_rank=true&hide=issues&border_radius=6&bg_color=00000000&border_color=30363d&text_color=8b949e&icon_color=58a6ff" />

---

<sub>认可并感谢 [LINUX DO](https://linux.do) 社区。</sub>
