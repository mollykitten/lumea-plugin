# Lumea — плагин для Claude Code

Публичный маркетплейс плагина `lumea` (Lumea — CRM поддержки; адрес сервера и ключ выдаёт администратор). Версия плагина совпадает с версией сервера; репозиторий обновляется автоматически с каждым релизом.

```
/plugin marketplace add mollybyte/lumea-plugin
/plugin install lumea@lumea
```

Адрес сервера Lumea сообщает администратор и задаётся переменной `LUMEA_URL`; ключ доступа выпускается в Lumea (Настройки → «Ключи доступа») и задаётся переменной `LUMEA_ACCESS_KEY` — обе обязательны. Подробности, список скиллов и проверка — [plugins/lumea/README.md](plugins/lumea/README.md).

Обновление: `/plugin marketplace update lumea`, затем `/plugin update lumea`.

## DeepSeek Harness (dsh)

Тот же каталог — бандл для [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness): MCP-сервер Lumea, скиллы и хуки-предохранители.

```
dsh plugin --profile <профиль> add github:mollybyte/lumea-plugin#v0.56.2
export LUMEA_URL=https://<адрес Lumea>
export LUMEA_ACCESS_KEY=lmk_…
```

Ограничения, проверка и переменные — в разделе «DeepSeek Harness» файла [plugins/lumea/README.md](plugins/lumea/README.md).

Текущая версия: **0.56.2**.
