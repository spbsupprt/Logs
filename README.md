# Logs
Logs


- поднимаем 2 машины web и log

- на web поднимаем nginx

- на log настраиваем центральный лог сервер на любой системе на выбор

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


Генерируем логи и ошибки:

curl localhost && rm -rf /var/www/index.nginx-debian.html && curl localhost


Финальная проверка:

![image](https://github.com/user-attachments/assets/0cf0f29d-eab1-4a74-9c75-fd8a6f75b233)

![image](https://github.com/user-attachments/assets/1036f884-5276-497f-a709-f88b1f63bcd7)
