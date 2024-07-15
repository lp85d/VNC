Обновляем пакеты в Termux:
```pkg update && pkg upgrade```
Устанавливаем proot-distro:
```pkg install proot-distro```
Устанавливаем Debian:
proot-distro install debian
Входим в него:
proot-distro login debian
Обновляем:
apt update
Устанавливаем vncserver:
apt install tightvncserver
Установка окружения или рабочего стола:
apt install lxde --no-install-recommends
или:
apt install icewm xterm
Вводим:
vncserver
Задаем пароль, потом когда спросят -> нажать n
Запустить сервер:
vncserver

Выключить сервер:
vncserver -kill :1

Запустить с определенным разрешением:
vncserver -geometry WxH
Где W — ширина, а H — высота.
Входим в клиент VNC.
Адрес: localhost:1
Пароль: который в шаге 10
По желанию:
apt install firefox-esr neofetch
