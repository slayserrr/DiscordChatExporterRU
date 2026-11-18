# DiscordChatExporter

[![Status](https://img.shields.io/badge/status-maintenance-ffd700.svg)](https://github.com/Tyrrrz/.github/blob/prime/docs/project-status.md)
[![Build](https://img.shields.io/github/actions/workflow/status/Tyrrrz/DiscordChatExporter/main.yml?branch=prime)](https://github.com/Tyrrrz/DiscordChatExporter/actions)
[![Coverage](https://img.shields.io/codecov/c/github/Tyrrrz/DiscordChatExporter/prime)](https://codecov.io/gh/Tyrrrz/DiscordChatExporter)
[![Release](https://img.shields.io/github/release/Tyrrrz/DiscordChatExporter.svg)](https://github.com/Tyrrrz/DiscordChatExporter/releases)
[![Downloads](https://img.shields.io/github/downloads/Tyrrrz/DiscordChatExporter/total.svg)](https://github.com/Tyrrrz/DiscordChatExporter/releases)
[![Pulls](https://img.shields.io/docker/pulls/tyrrrz/discordchatexporter)](https://hub.docker.com/r/tyrrrz/discordchatexporter)
[![Discord](https://img.shields.io/discord/869237470565392384?label=discord)](https://discord.gg/2SUWKFnHSm)

<table>
    <tr>
        <td width="99999" align="center">Разработка этого проекта полностью финансируется сообществом. <b><a href="https://tyrrrz.me/donate">Рассмотрите возможность поддержать проект пожертвованием!</a></b></td>
    </tr>
</table>

<p align="center">
    <img src="favicon.png" alt="Icon" />
</p>

**DiscordChatExporter** — это приложение, которое можно использовать для экспорта истории сообщений из любого канала [Discord](https://discord.com) в файл.
Оно работает с личными сообщениями, групповыми сообщениями и каналами серверов, а также поддерживает диалект markdown, используемый в Discord, и большинство других возможностей работы с форматированным и мультимедийным содержимым.

> [!WARNING]
> Хотя **DiscordChatExporter** это позволяет, автоматизация пользовательских аккаунтов нарушает TOS Discord и может привести к блокировке.
> По возможности используйте бота для экспорта журналов чата из доступных каналов.

**См. также**:
- 📦 [mlomb/chat-analytics](https://github.com/mlomb/chat-analytics) — решение для анализа шаблонов общения пользователей Discord на основе экспортов, созданных **DiscordChatExporter**
- 📦 [slatinsky/DiscordChatExporter-frontend](https://github.com/slatinsky/DiscordChatExporter-frontend) — удобная программа просмотра для экспортов, созданных **DiscordChatExporter**

## Скачать

- **Графический интерфейс** (настольное приложение):
  - 🟢 **[Стабильный релиз](https://github.com/Tyrrrz/DiscordChatExporter/releases/latest)**: ищите `DiscordChatExporter.*.zip`
  - 🟠 [CI-сборка](https://github.com/Tyrrrz/DiscordChatExporter/actions/workflows/main.yml): ищите `DiscordChatExporter.*.zip`
  - 📦 [Scoop](https://scoop.sh/#/apps?q=DiscordChatExporter&p=1&id=c71b7367623c560a2dc746b9739b9568b79b59ae): `scoop install extras/discordchatexporter` (поддерживается сообществом)
  - 📦 [WinGet](https://winstall.app/apps/Tyrrrz.DiscordChatExporter.GUI): `winget install Tyrrrz.DiscordChatExporter.GUI` (поддерживается сообществом)
  - 📦 [AUR](https://aur.archlinux.org/packages/discord-chat-exporter-gui): `yay -S discord-chat-exporter-gui` (поддерживается сообществом)
  - 📦 [Nix](https://search.nixos.org/packages?show=discordchatexporter-desktop): `nix-shell -p discordchatexporter-desktop` (поддерживается сообществом)
- **Интерфейс командной строки** (терминальное приложение):
  - 🟢 **[Стабильный релиз](https://github.com/Tyrrrz/DiscordChatExporter/releases/latest)**: ищите `DiscordChatExporter.Cli.*.zip`
  - 🟠 [CI-сборка](https://github.com/Tyrrrz/DiscordChatExporter/actions/workflows/main.yml): ищите `DiscordChatExporter.Cli.*.zip`
  - 🐋 [Docker](https://hub.docker.com/r/tyrrrz/discordchatexporter): `docker pull tyrrrz/discordchatexporter`
  - 📦 [WinGet](https://winstall.app/apps/Tyrrrz.DiscordChatExporter.CLI): `winget install Tyrrrz.DiscordChatExporter.CLI` (поддерживается сообществом)
  - 📦 [AUR](https://aur.archlinux.org/packages/discord-chat-exporter-cli): `yay -S discord-chat-exporter-cli` (поддерживается сообществом)
  - 📦 [Nix](https://search.nixos.org/packages?show=discordchatexporter-cli): `nix-shell -p discordchatexporter-cli` (поддерживается сообществом)

> [!NOTE]
> Пакеты, поддерживаемые сообществом, публикуются независимо от этого репозитория и могут не всегда соответствовать последнему релизу.

> [!NOTE]
> Если вы не уверены, какая сборка подходит для вашей системы, воспользуйтесь [этой страницей](https://useragent.cc), чтобы определить вашу ОС и архитектуру процессора.

## Возможности

- Кроссплатформенный графический интерфейс и интерфейс командной строки
- Аутентификация с помощью токена пользователя или бота
- Несколько форматов вывода: HTML (тёмная/светлая тема), TXT, CSV, JSON
- Поддержка markdown, вложений, embed-блоков, эмодзи и других возможностей работы с форматированным и мультимедийным содержимым
- Разбиение на файлы, диапазоны дат, фильтрация сообщений и другие параметры экспорта
- Автономные экспорты, которые можно просматривать офлайн
