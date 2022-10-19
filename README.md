# TMDB_api
Программа создает создает подборку фильмов через сервис TMDB по заданным параметрам, таким как жанр, бюджет картины, язык. На основе интересующих пользователя фильмов из его библиотеки проводится сравнение с результами, полученными с сервиса и формируется рекомендательный список. 

## requirements.txt

В файле указаны требования к версиям библиотек.

## LICENSE

Файл с указанием лицензии.

## .gitignore

Файл, в который вносятся исключения для отображения в коммитах и репозитории.

## tmdb_helpers.py

Файл содержит является вспомогательным для `hello_api_TMDB.py`. Он содержит параметры запросов и запрашивает пользователя ввести токен для работы с API. 

## search_in_db.py

Запрашивает у пользователя директорию, в которой находятся фильм и их названия. Проводит проверку, есть ли в директории информация о фильме, введеном пользователем. На основе полученных данных производится сортировка списка фильмов.

## own_db_helpers.py

Находит по заданному пользователем пути файл и загружает данные о нем в формате json.

## make_own_db.py

Загружает данные о большом количестве случайных фильмов и объединяет их с теми, что ввел пользователь.

## hello_api_TMDB.py

Получает ключ TMDB_API и делает запрос по выбранному номеру фильма. Если токен является неверным, скрипт сообщит об ошибке.

## find_similar.py

Производит поиск совпадений фильмов загруженных с сервиса и объявленных пользователем. При наличии в списке фильма, введеного пользователем, проводится проверка на соответствие объявленым параметрам, а именно язык, бюджет и жанр. На этой основе формируется финальный список рекомендаций и выводится пользователю в отсортированным виде.

## Как запустить

Для того, чтобы запустить скрип, необходим через командную строку ввести команду, находясь в директории с проектом
```
python main.py
```
