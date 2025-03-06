# Сгенерируйте конфиг Cloudflare WARP для Husi v0.10.12

## Aeza Terminator
Этот bash скрипт сгенерирует конфиг Cloudflare WARP для Husi v0.10.12.

Не стоит выполнять его локально, так как РКН заблокировал запросы для получения конфига. Вместо этого лучше выполнять на удалённых серверах.

1. Заходим на https://terminator.aeza.net/en/
2. Выбираем **Debian**
3. Вставляем команду:

```bash
bash <(wget -qO- https://raw.githubusercontent.com/AlexDon228/bash-warp-generator/refs/heads/main/warp_generator_husi.sh)
```
4. После того, как конфиг сгенерируется скачиваем файлом по ссылке.

5. Импортируем содержимое файла в Husi v0.10.12 через меню Пользовательская конфигурация.

Что-то не получилось? Есть вопросы?

Пишите в [Husi на 4pda](https://4pda.to/forum/index.php?showtopic=1083801) 
