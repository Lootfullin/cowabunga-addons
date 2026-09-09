# CowabungaAddons

Общий каталог плагинов Cowabunga для Jellyfin, независимый от репозиториев отдельных плагинов.

В **Панель управления → Плагины → Репозитории** добавьте название **CowabungaAddons** и адрес:

```text
https://raw.githubusercontent.com/Lootfullin/cowabunga-addons/main/manifest.json
```

Если каталог уже подключён через `jellyfin-smart-resolver`, замените старый URL новым. Удалять установленные плагины для смены URL не требуется.

| Плагин | Jellyfin | Исходники и релизы |
| --- | --- | --- |
| Cowabunga Jellyfin Companion | 12.0 | [Репозиторий](https://github.com/Lootfullin/cowabunga-jellyfin-companion) |
| Jellyfin Smart Resolver | 10.11.11 | [Репозиторий](https://github.com/Lootfullin/jellyfin-smart-resolver) |
| Choose your Meta! | 10.11.11 | [Репозиторий](https://github.com/Lootfullin/choose-your-meta) |
| Cowabunga Custom Artwork | 10.11 | [Репозиторий](https://github.com/Lootfullin/jellyfin-custom-artwork) |

Companion объединяет три модуля. Порядок импорта настроек и удаления прежних плагинов описан в его README. Старые плагины не заменяются автоматически на Companion: у него отдельный GUID.

## Обновление каталога

Сначала опубликуйте ZIP в релизе соответствующего плагина, затем обновите `versions` в `manifest.json`: версию, `targetAbi`, URL, дату и MD5 **опубликованного ZIP**. Сохраняйте GUID плагинов и совместимые предыдущие версии. SHA-256 дополнительно публикуется с релизом Companion.
