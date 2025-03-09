# Сгенерируйте конфиг Cloudflare WARP для Husi

## Forker from

[ImMALWARE/bash-warp-generator](https://github.com/ImMALWARE/bash-warp-generator)

[DikozImpact/bash-warp-generator](https://github.com/DikozImpact/bash-warp-generator)

### Aeza Terminator
Этот bash скрипт сгенерирует конфиг Cloudflare WARP для Husi v0.10.12.

Не стоит выполнять его локально, так как РКН заблокировал запросы для получения конфига. Вместо этого лучше выполнять на удалённых серверах.

1. Заходим на https://terminator.aeza.net/en/
2. Выбираем **Debian**
3. Вставляем команду:

```bash
bash <(wget -qO- https://raw.githubusercontent.com/AlexDon228/bash-warp-generator/refs/heads/main/warp_generator_husi.sh)
```
4. После того, как конфиг сгенерируется скачиваем файл по ссылке.

На Android нужно 2 раза на ссылку нажать, и потом зажать, тогда появится вариант скопировать. Лучше в Хроме делать, Яндекс баганный.

5. По умолчанию конечная точка прописана:
- адрес: XXXXXXXXXXXX
- порт: XXXX

Заменяем на значения, работающие у вашего провайдера.

6. В новом шаблоне WARP добавил параметры:
- Прослушиваемый порт:
"listen_port": 0
- Интервал постоянного поддержания активности WireGuard, в секундах:
"persistent_keepalive_interval": 600

Можете изменить на свои значения, либо вообще удалить.
7. Импортируем файл конфигурации WARP в Husi.

Что-то не получилось? Есть вопросы?

Пишите в теме [Husi на 4pda](https://4pda.to/forum/index.php?showtopic=1083801) 
