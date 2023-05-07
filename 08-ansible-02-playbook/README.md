# Домашнее задание к занятию 2 «Работа с Playbook»

## Подготовка к выполнению

1. * Необязательно. Изучите, что такое [ClickHouse](https://www.youtube.com/watch?v=fjTNS2zkeBs) и [Vector](https://www.youtube.com/watch?v=CgEhyffisLY).
2. Создайте свой публичный репозиторий на GitHub с произвольным именем или используйте старый.
3. Скачайте [Playbook](./playbook/) из репозитория с домашним заданием и перенесите его в свой репозиторий.
4. Подготовьте хосты в соответствии с группами из предподготовленного playbook.

## Основная часть

1. Подготовьте свой inventory-файл `prod.yml`.
2. Допишите playbook: нужно сделать ещё один play, который устанавливает и настраивает [vector](https://vector.dev).
3. При создании tasks рекомендую использовать модули: `get_url`, `template`, `unarchive`, `file`.
4. Tasks должны: скачать дистрибутив нужной версии, выполнить распаковку в выбранную директорию, установить vector.
5. Запустите `ansible-lint site.yml` и исправьте ошибки, если они есть.
6. Попробуйте запустить playbook на этом окружении с флагом `--check`.
7. Запустите playbook на `prod.yml` окружении с флагом `--diff`. Убедитесь, что изменения на системе произведены.
8. Повторно запустите playbook с флагом `--diff` и убедитесь, что playbook идемпотентен.
9. Подготовьте README.md-файл по своему playbook. В нём должно быть описано: что делает playbook, какие у него есть параметры и теги.
10. Готовый playbook выложите в свой репозиторий, поставьте тег `08-ansible-02-playbook` на фиксирующий коммит, в ответ предоставьте ссылку на него.

Ответ:

1.

<img width="350" alt="image" src="https://user-images.githubusercontent.com/5601009/236682719-1f6c9af9-e772-4749-8d2b-fc2b4854a1a1.png">

2-4.

<img width="548" alt="image" src="https://user-images.githubusercontent.com/5601009/236682776-e073aefd-6d64-4be6-9959-4f2da4535e78.png">

5.

<img width="500" alt="image" src="https://user-images.githubusercontent.com/5601009/236688920-8ca3e43d-b98a-4665-9bb7-1715f40d48a0.png">

6.

<img width="751" alt="image" src="https://user-images.githubusercontent.com/5601009/236690245-2dd3e5a0-e814-476c-8b5b-573e57931d30.png">

7.

<img width="751" alt="image" src="https://user-images.githubusercontent.com/5601009/236690384-12462ff2-5a8d-4d3e-b4bf-c1b1a1786025.png">

8.

<img width="751" alt="image" src="https://user-images.githubusercontent.com/5601009/236690508-e0397f76-1238-4a22-8bb8-89e071e2892f.png">

9.
Параметры:
1) Хендлеры - Старт сервисов clickhouse и vector
2) Таски - Скачивание пакетов установки сервисов, установки пакетов, создание базы

Тэги:
clickhouse & vector

---

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

---
