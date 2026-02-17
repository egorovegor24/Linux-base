---
order: 1.5
title: Не удалось получить информацию о компьютере
---

#### **Ошибка возникает при формировании протокола**

Пример ошибки:

<image src="./ne-udalos-poluchit-informaciyu-o-kompyutere.png" crop="0,0,100,100" scale="76" width="1920px" height="1080px" float="center"/>

Решение:

Выполните в терминале команду:

1. `sudo systemctl status gia11_cpd`  (данная команда отобразит текущий статус службы **gia11_cpd)**

2. `sudo systemctl start gia11_cpd`  (данная команда запустит службу **gia11_cpd)**

3. `sudo systemctl status gia11_cpd`  (данная команда отобразит текущий статус службы **gia11_cpd)**