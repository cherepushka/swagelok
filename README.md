# https://swagelok.su/

## Требования

- PHP >= 8.1

## Установка

- Скачать `MODX` с [официального сайта](https://modx.com/download) и выполнить его установку
- Добавить дамп базы данных в `MySQL`
- Инициализировать `git` внутри проекта
- Добавить в проект удалённый репозиторий с помощью команды `git remote add`
- Выполнить `git pull`
- Выполнить `composer install` и `npm install` для установки зависимостей
- Поменять настройки при необходимости в таблице `modx_system_settings`
- Переименовать файл `.htaccess.example` в `.htaccess`
- Скопировать файл `.env.example` и переименовать копию в `.env`.

## DEV информация

- `scss` файлы собираются через `webpack.mix`
- Для запуска сборщика `css,js` файлов используйте команду `npm run dev` или `npm run watch`
- Все исходные (до компиляции) `js` файлы находятся в `assets/resources/js`
- Все исходные (до компиляции) `css` файлы находятся в `assets/resources/scss/`

## Перенос изменений с локального сервера на боевой с помощью `git` (все данные для входа присутствуют в .xlsx файле)

- С помощью терминала подключаемся по `ssh` к хосту
- Выполняем `git` команды