# :radio_button: Тестовое задание full stack Aeon
## :two: PHP/JS

:pencil: Скачать тестовый проект: [https://github.com/atr-one/full-stack](https://github.com/atr-one/full-stack)

Авторизация по любому из номеров телефонов в таблице users, код подтверждения 1111. В проекте сейчас только одна вкладка Plots (раздел с участками, где выводится краткая информация о них и функционал редактирования). Надо добавить второй раздел Users (пользователи) с аналогичным функционалом, где будет выводиться информация о владельцах участков и возможность отредактировать данные пользователя.

Требования:
- таблица Users с владельцами участков (колонки Plot ID, First name, Last Name, Phone, Email, Last login)
- пагинация по 20 записей на страницу (аналогично таблице Plots)
- поиск по номеру телефона, имени и email пользователя
- страница реализуется в схожем дизайне, как страница с Plots
- возможность создания/редактирования пользователя (поля First name, Last name, Phone, Email, Plots)
- должна поддерживаться возможность добавить пользователя сразу к нескольким участкам (через запятую в поле Plots)
- если при редактировании какие-либо поля, кроме Plots не заполнены, не давать сохранить данные
- при сохранении данных телефон фильтруется по нечисловым символам, email переводится в lower case
- в меню при выборе раздела Users он должен подсвечиваться аналогично выбору Plots
- возможность удаления пользователя

## :hammer_and_wrench: Развертывание проекта в докере

```shell
docker compose -f ./docker/docker-compose.yaml up -d --build
```
