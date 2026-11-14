## 🇷🇺 Русский

### ✨ Обзор
Windows 10 и 11 по умолчанию не поддерживают полные флаговые эмодзи Unicode (например 🇻🇳 🇺🇸 🇯🇵 🇫🇷 🇩🇪). Этот репозиторий предлагает полное решение для исправления системы и корректного отображения флагов во всех приложениях.

Без ожидания обновлений от Microsoft. Без полумер. Это техническое решение от Tuannvbg — разработчика из Вьетнама, сделавшего всё, чтобы флаги отображались правильно.

## 🦊 Глобальный вызов: исправить отображение эмодзи-флагов в Firefox
[![Вызов Emoji-флагов Firefox](https://img.shields.io/badge/Firefox_Emoji_Флаги-🚩_Исправь_и_прославься-red)](guides/firefox.prefix.ru.md)

## 📚 Руководство по установке
🌐 Просмотреть другие языковые версии:  
- 🇻🇳 [Tiếng Việt](./guides/windows.vi.md)
- 🇺🇸 [English version](./guides/windows.en.md)
- 🇨🇳 [中文版本 (China)](./guides/windows.zh.md)
- 🇷🇺 [Русская версия (Russia)](./guides/windows.ru.md)
- 🌐 [Other languages](./guides/) (coming soon)

## 🧪 Матрица совместимости

## 🌍 Emoji Picker, Unicode 17.0 — Техническое открытие о модификации emoji-флагов для Windows 10

### ✅ Рекомендуемая инструкция по установке

Это интересное открытие: установив шрифт `Segoe.UI.Emoji.with.Twemoji.Flags.ttf`, я получил возможность:

- Использовать emoji-панель в стиле Windows 11  
- Полноценно отображать emoji из Unicode 17.0 (🫨🫠🫷🫸)  
- Отображать цветные emoji-флаги стран (🇻🇳🇺🇸🇯🇵)

---

### 🔹 Шаг 1: Ознакомьтесь с инструкцией 🇷🇺 [Русский](./guides/windows.ru.md)

### 🔹 Шаг 2: Установите шрифт, поддерживающий emoji-флаги

📁 Шрифт: [`Segoe.UI.Emoji.with.Twemoji.Flags.ttf`](https://github.com/Chasmical/flag-emojis-for-windows)  
📁 Или загрузите из: [`/fonts/`](https://github.com/tuannvbg/unicode-flags-for-windows/tree/main/fonts)

- ✅ Отображает цветные emoji-флаги (например: 🇯🇵🇫🇷🇧🇷)  
- ✅ Работает с emoji-панелью Windows (`Win + .`)  
- 🧩 Основан на Segoe UI Emoji v1.60 и дополнен Twemoji v16.0.1  
- 📌 Этот шрифт дополняет базовый — не заменяет его полностью

---

### 🔍 Технический анализ: объединение шрифтов для расширения поддержки emoji

Шрифт `seguiemj_1_31_mod.ttf` уже поддерживает emoji-флаги, но так как он основан на оригинальном шрифте Windows 10, визуальный стиль emoji устаревший — не такой современный, как Fluent 3D в Windows 11.

→ Поэтому я попробовал установить `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` от Chasmical, чтобы:

- ✅ Сохранить цветные emoji-флаги  
- ✅ Получить визуальный стиль emoji, как в Windows 11 (на базе Segoe UI Emoji v1.60)  
- ✅ Совместить с `seguiemj_1_31_mod.ttf` для поддержки Unicode 17.0 (🫨🫠🫷🫸)

📌 Технические детали:

- Шрифт Chasmical не заменяет все emoji — он добавляет только 258 emoji-флагов из Twemoji v16.0.1  
- Остальные emoji взяты из Segoe UI Emoji v1.60 — Fluent 3D 15.1 (Windows 11 23H2, дата: 25 июня 2024)  
- Из репозитория Chasmical:

  > *“Этот шрифт основан на Segoe UI Emoji v1.60 (3D Fluent 15.1; Win11 23H2; 2024-06-25) и содержит 258 флагов из Twitter Color Emoji SVGinOT v16.0.1 (2025-04-14), собранных quarrel.”*

🧠 Установив сначала `seguiemj_1_31_mod.ttf`, система использует его как fallback для отображения emoji из Unicode 17.0, которых нет в шрифте Chasmical.  
→ Это умная стратегия объединения шрифтов:  
- Первый шрифт — для новых символов Unicode  
- Второй — для современного визуального стиля и флагов  
→ В результате Windows 10 отображает emoji как Windows 11 — но даже лучше, с поддержкой Unicode 17.0.

---

### 📷 Настройка шрифта в браузере для корректного отображения emoji-флагов

После установки `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` я настроил браузер, чтобы emoji-флаги отображались в цвете.

✅ Совет: используйте `'Noto Color Emoji'` вместо `'Segoe UI Emoji'`, чтобы избежать синеватых или отсутствующих флагов.

---

### 📸 Примеры отображения

#### 🧩 Emoji-панель Windows 11 в Windows 10

![Emoji-панель Windows 11 в Windows 10](./screenshots/win10/Win10.Emoji.Picker.Style.Win11.p2.20250930.JPG)

---

#### 🌐 Chrome после настройки `'Noto Color Emoji'`

![Флаги в Chrome](./screenshots/win10/Win10.Chrome.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🌐 Edge после настройки `'Noto Color Emoji'`

![Флаги в Edge](./screenshots/win10/Win10.Edge.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🔍 Chrome на сайте emojipedia.org — тест Unicode 17.0

![Chrome на emojipedia.org](./screenshots/win10/Win10.Chrome.blog.emojipedia.org.20250930.JPG)

### 🧪 Таблица совместимости

| ОС + Шрифт | Unicode 17.0 | Emoji-флаги | Примечание |
|--------------------------|----------------|------------------|-------------|
| Win10 + `seguiemj_1_31_mod.ttf` | ✅ | ✅ | Полный набор emoji, но устаревший стиль |
| Win10 + `seguiemj_1_31_mod.ttf` + Twemoji Flags | ✅ | ✅ | Полный набор emoji с современным стилем |
| Win11 + только Twemoji Flags | ❌ | ✅ | Только флаги, нет поддержки Unicode 17.0 |

---

### 📢 Заключение

✅ **Windows 10 полностью поддерживает Unicode 17.0 и цветные emoji-флаги**,  
если установить шрифты в правильном порядке: **сначала базовый**, **затем Twemoji Flags**,  
и настроить браузер на использование `'Noto Color Emoji'` для корректного отображения флагов.

| ОС + Шрифт | Emoji Unicode 17.0 | Флаги emoji | Примечание |
|------------|---------------------|--------------|------------|
| Windows 10 + `seguiemj_1_31_mod.ttf` | ✅ | ✅ | Идеальное сочетание — поддержка всех emoji |
| Windows 11 + `seguiemj_1_33_mod.ttf` | ❌ | ✅ | Флаги отображаются, но нет новых emoji |
| Windows 11 + только Twemoji Flags | ❌ | ✅ | Есть цветные флаги, нет Unicode 17.0 emoji |
> Эта таблица показывает, какие функции emoji поддерживаются в разных версиях Windows при использовании модифицированных шрифтов.


> Firefox всё ещё неправильно отображает эмодзи-флаги Unicode.  
> Тот, кто решит проблему, будет внесён в [Стену славы Firefox](guides/firefox.wall-of-fame.ru.md) 🏅

- 🌍 [Посмотреть вызов](guides/firefox.prefix.ru.md)  
- 🛠️ [Отправить своё решение](guides/firefox.fix.template.ru.md)
## 🤔 Сравнение с другими решениями

Возможно, вы слышали о таких проектах, как:

- [`13rac1/twemoji-color-font`](https://github.com/13rac1/twemoji-color-font)
- Скрипты для внедрения кастомных emoji-шрифтов
- Замена emoji на SVG-изображения в браузере (Twemoji CDN и др.)

У каждого подхода есть свои плюсы и минусы.

| Критерий                   | twemoji-color-font         | unicode-flags-for-windows     |
|----------------------------|----------------------------|-------------------------------|
| Эмодзи-флаги отображаются правильно? | ⚠️ Возможно (зависит от системы) | ✅ Стабильно, Unicode по умолчанию |
| Цветные эмодзи?            | ❌ В основном чёрно-белые    | ✅ Полноцветные                 |
| Меняет системные шрифты?   | ❌ Нет                      | ✅ Да (с резервной копией)      |
| Оптимизация под Windows 10/11? | ❌ Не завершена            | ✅ Специально оптимизировано    |
| Требуется правка реестра?  | ❌ Нет                      | ✅ Да (авто / вручную)          |
| Поддержка Firefox?         | ❌ Не целевая платформа     | ❓ (текущий вызов)              |
| Активность сообщества?     | ✅ Довольно активное         | 🆕 Только стартовало            |

📣 Хотите помочь Firefox правильно отображать эмодзи-флаги?  
→ [Примите участие в вызове](guides/firefox.prefix.ru.md) 🦊🔥

## 📸 Скриншоты

### ✅ Приложение Copilot PC
> Emoji-флаги корректно отображаются в приложении Copilot PC на Windows 11  
![Скриншот Copilot PC](screenshots/Copilot.PC.app.Windows11.Screenshot.2025-09-21.103357.jpg)

### ✅ Блокнот (Notepad)
> Даже самое простое приложение теперь правильно отображает Unicode-флаги  
![Скриншот Notepad](screenshots/Notepad.Screenshot.2025-09-21.103618.jpg)

### ✅ Visual Studio Code
> VS Code показывает emoji-флаги в markdown и комментариях к коду  
![Скриншот VS Code](screenshots/VSC2.Screenshot.2025-09-21.104033.jpg)

### ✅ Браузер Chrome
> Chrome идеально отображает emoji-флаги после установки патча  
![Скриншот Chrome](screenshots/Chrome.Browser.Show.Screenshot.2025-09-21.111129.jpg)

### ✅ Браузер Microsoft Edge
> Edge отображает emoji-флаги в Copilot Web и многоязычном контенте  
![Скриншот Edge](screenshots/Edge.Browser.Show.Screenshot.2025-09-21.111408.jpg)

### ✅ Браузер Firefox
> Firefox по-прежнему не может корректно отобразить Unicode emoji-флаги  
![Скриншот Firefox](screenshots/Firefox.Browser.Screenshot.2025-09-21.183410.jpg)

---

## 🙌 Благодарности

- [`Chasmical/flag-emojis-for-windows`](https://github.com/Chasmical/flag-emojis-for-windows)  
- [`perguto/Country-Flag-Emojis-for-Windows`](https://github.com/perguto/Country-Flag-Emojis-for-Windows)  
- [`llccd.eu.org`](https://llccd.eu.org/2022/02/win_flags)  
- [`13rac1/twemoji-color-font`](https://github.com/13rac1/twemoji-color-font)  
- Copilot AI — партнёр по техническому мозговому штурму

---

## 💬 Автор

Tuannvbg 🇻🇳 – Делает эмодзи флагов Unicode корректно отображаемыми в Windows 😎🇻🇳🇺🇸

---

## 📄 Лицензия

Этот проект распространяется по лицензии MIT — вы можете свободно использовать, изменять и делиться им, чтобы помочь обеспечить корректное отображение Unicode emoji-флагов в системах Windows.

