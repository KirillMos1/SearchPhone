<h1 align="center">SearchPhone 🕵🏽‍♂️ (FORK OF KIRILLMOS1)</h1>

<p align="center">
Это самоисчерпывающй OSINT-инструмент для поиска привязанной к телефону информации, используя несколько API доя сбора информации с различных источнков. Разработано на Python для CLI
</p>

<p align="center">
<img src="assets/SearchPhone.png" title="SearchPhone" alt="SearchPhone" width="600"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white" alt="Python version">
  <img src="https://img.shields.io/badge/NUMVERIFY/SERPAPI/GITHUB-API-blue?logo=rapidapi&logoColor=white">
  <img src="https://img.shields.io/badge/License-MIT-green?logo=open-source-initiative&logoColor=white" alt="License">
</p>

## ✨ Возможности

- 📱 **Проверка номера** - Проверяет и стандартизирует телефонный номер с помощью `phonenumbers`
- 🔍 **Поиск по нескольким сервисам** - Поиск по Google (с помощью SerpAPI), DDG (aka DuckDuckGo) и Bing
- 💻 **Поиск по репозиториям** - Поиск номера в Github репозиториях
- 📝 **Поиск в соцсетях** - Ищет упоминаня на Reddit
- 📊 **Геолокация (примерно)** - Ищет оператора и примерную локацию через Numverify API
- 📄 **Автосоздание отчета** - Генерация JSON и PDF результата поиска
- 🚀 **Парралельный поиск** - Ищет сразу по нескольким источникам для скорости
- 🎨 **Цветной вывод** - Удобный для чтения вывод с поддержкой цветов
- **Поддержка мультиязычности (добавлено в форке)** - Благодаря `locate.tmx` и переменной окружения `SEARCHPHONE_LANG` вы сможете установить язык для работы с утилитой

## 🔑 Необходимые API ключи

Получите API ключи через эти сервисы:

| Сервис | Для чего получать ключ | Ссылка | Лимиты | Необходимость |
|---------|---------|------|------|-----|
| **Numverify** | Проверка номера и передача информации о нем | [numverify.com](https://numverify.com/) | 100 запросов/месяц бесплатно | Обязателен |
| **SerpAPI** | Результаты поиска в Google | [serpapi.com](https://serpapi.com/) | 250 запросов/месяц бесплатно | Обязателен |
| **GitHub Token** | Поиск по Github | [GitHub Settings](https://github.com/settings/tokens) | 5000 запросов/месяц бесплатно | Обязателен |

### Настройка API ключей

Утилите нужен `.env` файл для задания необходимых переменн окружения. Выполните код (не в зависимости от вашей операционной системы)

```
echo "NUMVERIFY_KEY=<ваш ключ>" >> .env
echo "SERPAPI_KEY=<ваш ключ>" >> .env
echo "GITHUB_TOKEN=<ваш ключ>" >> .env
```

Файл [`example.env`](https://github.com/KirillMos1/SearchPhone/edit/main/example.env) можете спокойно удалить

> **Проект открыт для партнеров**

# Доступные ОС и диструбутивы
|ОС|Официальный релиз|Поддерживается|Статус|
|---|---|---|---|
|Kali Linux|2026.1a+|✅|Работает|
|Parrot Security OS|6.3|✅|Работает|
|Windows|10+|✅|Работает|
|BackBox|9|✅|Работает|
|Arch Linux|2024.12.01|✅|Работает|

> **Немного справки от KirillMos1**
>
> Данная утилта работает со всеми ОС, поддерживающими Python 3.8+

# Использование

Windows 10+ (при условии того, что Python есть в PATH)

```cmd
pip install -r requirements.txt
python search_phone.py
```

Linux-диструбутивы:

```bash
pip3 install -r requirements.txt
python3 search_phone.py
```

# Поддержка

Вопросы, предложения и багрепорты отправлять на [info@hackunderway.com](mailto:info@hackunderway.com)

Вопросы по переводу и добавленного функционала направлять на [neminer@rambler.ru](mailto:neminer@rambler.ru)

# Лицензия

Данные проект защищен по лицензии MIT

# 👨‍💻 Автор оргинальной утилиты

* [Victor Bancayan](https://www.offsec.com/bug-bounty-program/) - (**CEO [Hack Underway](https://hackunderway.com/)**)

## 🔗 Ссылки
[![Patreon](https://img.shields.io/badge/patreon-000000?style=for-the-badge&logo=Patreon&logoColor=white)](https://www.patreon.com/c/HackUnderway)
[![Web site](https://img.shields.io/badge/Website-FF7139?style=for-the-badge&logo=firefox&logoColor=white)](https://hackunderway.com)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/HackUnderway)
[![Jey Zeta](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/JeyZetaOficial/subscribe/)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@JeyZetaOficial)
[![Twitter/X](https://img.shields.io/badge/Twitter/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/JeyZetaOficial)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/hackunderway)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/JeyZeta)

## ☕️ Поддержика данного проекта

Если вам понравилась утилита, можете задонатить разработчику на кофе:

[![Buy Me a Coffee](https://img.shields.io/badge/-Buy%20me%20a%20coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/hackunderway)

Если вам понравился именно форк, можете направить деньги форкеру:

[DonationAlerts](donationalerts.com/r/kirillkasparyants)

## Личное мнение форкера на данную тулзу

У меня складывается такое ощущение, что тулза ИИшная. Ну README точно.

Из <img src="https://i.imgur.com/ngJCbSI.png" title="Perú"> сделано на <img src="https://i.imgur.com/NNfy2o6.png" title="Python"> с <img src="https://i.imgur.com/S86RzPA.png" title="Love"> от <font color="red">Victor Bancayan</font>

Форк сделан KirillMos1

© 2026
