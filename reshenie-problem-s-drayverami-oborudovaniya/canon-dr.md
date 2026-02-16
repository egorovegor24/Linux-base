---
order: 2
title: Canon DR-C230
---

## **Для Альт Образование:**

На данный момент решения нет

## **Для Astra Linux SE 1.8.4:**

1. Для настройки выполните последовательно команды:

   `sudo apt install dpkg-dev -y`

   `sudo apt -f install`

2. Установить пакет `sane-utils` и `libusb-0.1-4` командой:\
   `sudo apt install sane-utils libusb-0.1-4`

3. Сохраните, направленный во вложении, пакет драйвера:

   [cndrvsane-drc230_1.00-2_amd64.rar](./cndrvsane-drc230_1.00-2_amd64.rar)

4. Создать каталог `/usr/lib/sane` \
   `sudo mkdir -p /usr/lib/sane`

5. Установите пакет драйвера:\
   `sudo dpkg -i /*абсолютный путь*/cndrvsane-drc230_1.00-2_amd64.deb`

6. Выполните поиск устройств:\
   `sudo scanimage -L`

7. Убедиться, что в выводе присутствует имя устройства с упоминанием драйвера c`anondr.`

8. Выполнить тестовое сканирование через утилиту **fly-scan** "Сканирование".

9. В случае необходимости удаления драйвера выполнить команду:\
   `sudo apt purge cndrvsane-drc230`