# Hackintosh для HP Pavilion 15-n057sr

## 💻 Характеристики

| Название                | Описание                               |
|-------------------------|---------------------------------------|
| Процессор              | Intel® Core i5-4200U                  |
| Видеокарта (iGPU)      | Intel® HD Graphics 4400               |
| Видеокарта (dGPU)      | AMD Radeon HD 8670M                   |
| Звук                   | Realtek ALC269                        |
| Тачпад                 | Synaptics PS2                         |
| Wi-Fi                  | MediaTek MT7630E (заменён на Atheros AR9285 - AR5B95) |
| Ethernet               | Realtek                               |
| Bluetooth              | MediaTek MT7630E (в Atheros AR9285 отсутствует) |
| Камера                 | HP TrueVision HD                      |
| Картридер              | RTS5227 PCI Express                   |



## ✅ Работает (почти всё)

- [x] Тачпад
- [x] Карта USB-портов
- [x] Отображение заряда АКБ
- [x] Wi-Fi*
- [x] Ethernet
- [x] Звук и микрофон
- [x] Камера
- [x] Картридер
- [x] Видеокарта (iGPU)
- [x] CPU SpeedStep (macOS правильно управляет процессором)

\* Wi-Fi работает, если вы замените Wi-Fi-карту на указанную (Atheros AR9285) и установите OCLP (для macOS Monterey и выше). Если у вас такая же карта, скачайте файл **EFI_ARWIFI**.  
Дефолтный Wi-Fi MediaTek **НЕ работает** и **не будет работать** в macOS.



## 🍎 Поддерживаемые ОС

| Название              | Работает | Протестировано |
|-----------------------|----------|----------------|
| OS X 10.9 Mavericks  | ✅        | ❌             |
| OS X 10.10 Yosemite  | ✅        | ❌             |
| OS X 10.11 El Capitan| ✅        | ❌             |
| macOS 10.12 Sierra   | ✅        | ❌             |
| macOS 10.13 High Sierra | ✅    | ✅             |
| macOS 10.14 Mojave   | ✅        | ✅             |
| macOS 10.15 Catalina | ✅        | ❌             |
| macOS 11 Big Sur     | ✅        | ✅             |
| macOS 12 Monterey    | ✅        | ✅             |
| macOS 13 Ventura     | ✅        | ✅             |
| macOS 14 Sonoma      | ❌        | ❌             |
| macOS 15 Sequoia     | ❌        | ❌             |

Все не протестированные системы, указанные выше, **в теории** должны работать, но требуется тестирование. Если использовать версию **NOWIFI**, все эти системы запустятся и будут работать. Для macOS 13 Ventura и новее нужен патч графики.



## ❌ Не работает

- [ ] Видеокарта (dGPU) — карта поддерживается в Hackintosh, но только если отсутствует iGPU.



## 🔵 О загрузчике

Мой EFI работает на базе OpenCore версии 0.8.5.  
Я использовал SMBIOS **MacBookPro12,1** для установки macOS Monterey.  
Советую изменить SMBIOS с помощью **GenSMBIOS** — лучше всего использовать **MacBookPro11,1**.

- Если вы не меняли Wi-Fi-адаптер, скачайте файл: **EFI_NOWIFI**. (https://github.com/sashaMacos/HP-Pavilion-15-n057sr-Hackintosh/releases/download/EFI/EFI_NOWIFI.zip)
- Если у вас карта Atheros AR9285 (AR5B95), скачайте файл: **EFI_ARWIFI**. (https://github.com/sashaMacos/HP-Pavilion-15-n057sr-Hackintosh/releases/download/EFI/EFI_ARWIFI.zip)
