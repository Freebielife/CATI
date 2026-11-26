# Catizen Observatory

## О проекте и токене

Catizen указывает, что CATI — его utility-токен, выпущенный Catizen Limited, дочерней компанией Catizen Foundation Company.

Источники проверены 26 ноября 2026 года:

- [Официальный сайт Catizen](https://catizen.ai/)
- [Официальный whitepaper: токеномика CATI](https://docs.catizen.ai/usdcati-tokenomics)
- [Официальный whitepaper: Catizen Foundation](https://docs.catizen.ai/decentralized-organization)
- [Официальный Telegram-канал](https://t.me/CatizenAnn)

## Данные обсерватории

- Контракт TON: `EQD-cvR0Nz6XAyRBvbhz-abTrRC6sI5tvHvvpeQraV9UAAD7`
- Точность: 9 знаков
- Подтверждённые пулы с TON: STON.fi и DeDust
- Логотип в банере и изображение флага взяты из файла, предоставленного владельцем проекта.
- Снимок данных собран 26 ноября 2026 года. Сбор настроенных разделов завершился без ошибок; исторические данные сделок по четырём пулам пока неполные.

HTML самодостаточный: при отображении не требуются внешние скрипты, шрифты или изображения. Размер собранного `index.html` — 475 310 байт (лимит — 2 500 000 байт).

## Сборка и обновление

```bash
python3 -m scripts.refresh_observatory
python3 build.py
python3 verify.py
```

GitHub Actions проверяет сайт при изменениях в `main` и поддерживает ручной запуск обновления. Наличие расписания общего Cloudflare-планировщика для этого репозитория отдельно не подтверждено.
