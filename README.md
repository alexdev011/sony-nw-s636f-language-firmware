# Sony Walkman NW-S636F (Japan / ICX1127) — Russian Language Firmware (v1.12)

[Русский](#русский) | [English](#english)

---

&lt;a name=&quot;русский&quot;&gt;&lt;/a&gt;
## Русский

Кастомная прошивка (v1.12) для японской версии плеера **Sony Walkman NW-S636F** (платформа `ICX1127`), добавляющая поддержку русского языка и пункт/кнопку выбора языка в штатную оболочку **Sony Gemini**.

> **Внимание:** Прошивка предназначена **только для японских моделей серии NW-S63xF** (`NW-S636F`, `NW-S638F`, `NW-S639F`, `VID=0x054c`, `PID=0x038d`). Не используйте её на других моделях. Все действия вы выполняете на свой страх и риск.

### Что изменено
- **Русский язык в штатном интерфейсе:** пропатчен системный бинарник оболочки `/usr/local/bin/gemini-ICX1127` (добавлена локализация и доступ к выбору языка в меню).
- **Версия прошивки:** `1.12` (на базе оригинальной японской `1.11`), чтобы официальный установщик Sony корректно определял обновление.
- **Заводской функционал:** музыка, FM-радио, настройки звука и подключение к ПК по USB работают в штатном режиме.

### Содержимое
- `FWUpdater.exe`, `FWUpdaterCom.dll`, `FWUpdaterRes.dll` — официальный установщик Sony.
- `NW-S63XF.ini` — конфигурация целевых устройств (`NW-S636F`, `NW-S638F`, `NW-S639F`).
- `NW_WM_FW.UPG` — модифицированный образ прошивки.
- `license_*.txt` — лицензионные соглашения.
- *(Опционально)* Папка с оригинальной японской прошивкой `1.11`.

### Перед установкой
1. **Сделайте резервную копию** всей музыки и важных файлов с накопителя плеера на ПК.
2. Полностью зарядите аккумулятор плеера.
3. Убедитесь, что у вас японский **NW-S636F** (или совместимая модель `NW-S638F` / `NW-S639F`).
4. При подключении к ПК **не соглашайтесь на форматирование** памяти плеера.

### Инструкция по установке
1. Скачайте файлы прошивки и распакуйте их в папку без кириллицы и пробелов в пути (например, `C:\NW-S636F-RU\`).
2. Подключите плеер к ПК по USB и закройте сторонние программы (SonicStage, Content Transfer и т.п.).
3. Запустите **`FWUpdater.exe`**, следуйте подсказкам на экране и **не отключайте кабель** до завершения процесса и перезагрузки.
4. После перезагрузки выберите нужный язык в настройках плеера.

### Смена региона (опционально)
На японских плеерах нет европейского лимита громкости, но FM-диапазон ограничен частотами 76–90 МГц. Для смены региона (Destination) можно использовать утилиту **`scsitool-nwz`** из проекта Rockbox. Подробнее: [Rockbox SonyNWDestTool](https://www.rockbox.org/wiki/SonyNWDestTool).

---

&lt;a name=&quot;english&quot;&gt;&lt;/a&gt;
## English

Custom firmware (v1.12) for the Japanese **Sony Walkman NW-S636F** (`ICX1127` platform) that adds Russian language support and a language selection option to the stock **Sony Gemini** shell.

> **Warning:** This firmware is intended **only for Japanese NW-S63xF series models** (`NW-S636F`, `NW-S638F`, `NW-S639F`, `VID=0x054c`, `PID=0x038d`). Do not flash it onto other models. Proceed at your own risk.

### Changes
- **Russian UI Localization:** Patched `/usr/local/bin/gemini-ICX1127` to add Russian localization and language switching support in the stock menu.
- **Firmware Version:** Bumped to `1.12` (based on stock Japanese `1.11`) so the official Sony updater accepts the package.
- **Stock Features Preserved:** Audio playback, FM tuner, sound settings, and USB mass storage remain fully functional.

### Package Contents
- `FWUpdater.exe`, `FWUpdaterCom.dll`, `FWUpdaterRes.dll` — official Sony firmware updater.
- `NW-S63XF.ini` — target device configuration (`NW-S636F`, `NW-S638F`, `NW-S639F`).
- `NW_WM_FW.UPG` — patched firmware image.
- `license_*.txt` — license agreements.
- *(Optional)* Original Japanese `1.11` firmware folder.

### Before Flashing
1. **Back up** all music and personal files from the player to your PC.
2. Fully charge the player's battery.
3. Verify your device is a Japanese **NW-S636F** (or compatible `NW-S638F` / `NW-S639F`).
4. Do **not** format the player's storage if Windows prompts you to do so.

### Installation
1. Download and extract the firmware files into a simple folder path without spaces or non-ASCII characters (e.g., `C:\NW-S636F-RU\`).
2. Connect the player via USB and close any Walkman management software (SonicStage, Content Transfer, etc.).
3. Run **`FWUpdater.exe`**, follow the on-screen instructions, and **do not disconnect the USB cable** until the update finishes and the player reboots.
4. Once rebooted, select your preferred language in the player's settings menu.

### Region Change (Optional)
Japanese units do not have the European volume cap, though the FM tuner is limited to 76–90 MHz. You can change the destination/region using **`scsitool-nwz`** from the Rockbox project. See the [Rockbox SonyNWDestTool](https://www.rockbox.org/wiki/SonyNWDestTool) documentation for details.

---

## References & Disclaimer / Ссылки и отказ от ответственности

- Sony Open Source Linux 2.6.10 kernel sources for NW-S636F: [oss.sony.net](https://oss.sony.net/Products/Linux/Audio/NWZ-S636F.html)
- Rockbox `scsitool` / `SonyNWDestTool`: [rockbox.org/wiki/SonyNWDestTool](https://www.rockbox.org/wiki/SonyNWDestTool)

This firmware is provided "as is" without warranty of any kind. You are solely responsible for any data loss or device damage.

- Sony Open Source Linux 2.6.10 kernel sources for NW-S636F: [oss.sony.net](https://oss.sony.net/Products/Linux/Audio/NWZ-S636F.html)
- Rockbox `scsitool` / `SonyNWDestTool`: [rockbox.org/wiki/SonyNWDestTool](https://www.rockbox.org/wiki/SonyNWDestTool)

This firmware is provided "as is" without warranty of any kind. You are solely responsible for any data loss or device damage.
