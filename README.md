# БОТ ДЛЯ ГЕМБЛИНГА
## [Пример](https://t.me/mines_aisignals_bot)

## Инструкция по настройке бота:
1. Создать бота, через BotFather
2. Создать телеграм канал и создать к нему чат
3. Сделать бота админом этого канала и канала, в котором он должен проверять подписку
4. В партнерке, создать постбэк и вставить ссылку `https://api.telegram.org/bot<TOKEN>/sendMessage?chat_id=<KANAL_ID>&text={sub1}`
	- TOKEN заменить на токен бота
	- KANAL_ID заменить на **id на созданный во 2 пункте канал**
5. В `config.py` заполнить значения:
	- BOT_TOKEN - токен бота, полученный через BotFather
	- CHANNEL_URL - ссылка на канал для проверки подписки, **именно ссылка**
	- CHANNEL_ID - id канала для проверки подписки, можно получить через ботов для получения id, пример `-123456778657`
	- VERIF_CHANNEL_ID - id чата для верификации, **именно чата а не канала**, можно получить там же, пример `-123456778657`
	- SUPP - ссылка на аккаунт поддержки, **именно ссылка**
	- ADMIN_ID - id пользователя, пример `1232423123`
	- PROMO - промокод из партнерки, будет вставляться в текст
6. Запустить бота локально и с помощью `/admin`, поменять ссылку на свою
7. Задеплоить на сервер
