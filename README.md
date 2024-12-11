# bottec

Описание сервисов находятся в:
```commandline
tg_bot_service/README.md
admin_panel_service/README.md
```

Файлы с переменными окружения (используются файлы без точки в начале):
```commandline
tg_bot_service/settings/env
admin_panel_service/admin_settings/env
```

При запуске БД должна заполниться тестовыми данными и в `/app/static_content/mailing_images` должны создасться 10 изображений
`/app/static_content/mailing_images` - общий вольюм для двух сервисов, через него происходит передача изображений от админки к боту

Так же для админки создается пользователь по умолчанию
```
admin panel:
host 0.0.0.0:8000
login: admin
password: admin
```

### Запуск:
```commandline
git clone git@github.com:trteo/bottec.git
git submodule update --init
docker-compose up --build
```