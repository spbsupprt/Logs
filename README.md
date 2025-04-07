# Logs
Logs


- поднимаем 2 машины web и log

- на web поднимаем nginx

- на log настраиваем центральный лог сервер на любой системе на выбор

- journald;

- rsyslog;

- настраиваем аудит, следящий за изменением конфигов нжинкса

- Все критичные логи с web должны собираться и локально и удаленно.

- Все логи с nginx должны уходить на удаленный сервер (локально только критичные).

Логи аудита должны также уходить на удаленную систему.

---

Дано:

![image](https://github.com/user-attachments/assets/41425ee8-f1ca-44a6-818b-fd3fbe7664b6)


Готовим конфигурационные файлы:

https://github.com/spbsupprt/Logs/tree/main/src

Пишем плейбук и применяем:

https://github.com/spbsupprt/Logs/blob/main/log.yml

![image](https://github.com/user-attachments/assets/882b3d0a-0414-4d27-8c92-0e4fd2125684)

Финальная проверка:

