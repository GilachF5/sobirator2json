# Source missing

Исходный код этой функции пока не восстановлен.

Что уже выгружено из Yandex Cloud:

- ID функции: `d4e4vojdhckor1ftecls`
- Runtime: `nodejs22`
- Entry point: `index.handler`
- Метаданные функции: `function.json`
- Метаданные версий: `versions.json`
- README с параметрами запуска: `README.md`

Почему здесь нет файлов `index.js` / `index.py`:

Yandex Cloud CLI и REST API для Cloud Functions отдают параметры функции и версии, но не отдают архив исходного кода уже созданной версии. В документации Yandex Cloud указано, что backup кода функции не хранится.

Что нужно найти, чтобы восстановить код:

- старую локальную папку проекта;
- ZIP/TAR, который загружался при деплое;
- объект в Yandex Object Storage, если деплой шел из бакета;
- старый GitHub/другой репозиторий;
- код из веб-редактора Yandex Cloud Console, если он там еще отображается.

Переменные окружения последней версии, без значений:

- `GOOGLE_PRIVATE_KEY`
- `GOOGLE_SERVICE_ACCOUNT_EMAIL`
- `SHEET_ID`

Реальные секреты не добавлялись в репозиторий.