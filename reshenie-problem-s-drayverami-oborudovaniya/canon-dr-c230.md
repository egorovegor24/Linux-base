---
order: 2.5
title: Canon DR-C225
---

## **Для Альт Образование:**

<highlight color="mint-green">***На данный момент решения нет***</highlight>

## **Для Astra Linux SE 1.8.4:**

1. Для настройки выполните последовательно команды:

   `sudo apt install dpkg-dev -y`

   `sudo apt -f install`

2. Установить пакет `sane-utils` и `libusb-0.1-4` командой:\
   `sudo apt install sane-utils libusb-0.1-4`

3. Сохраните, направленный во вложении, пакет драйвера:

   [cndrvsane-drc225_1.00-4_amd64.rar](./cndrvsane-drc225_1.00-4_amd64.rar)

4. Создайте каталог `/usr/lib/sane` \
   `sudo mkdir -p /usr/lib/sane`

5. Установите пакет драйвера:\
   `sudo dpkg -i /*абсолютный путь*/cndrvsane-drc230_1.00-2_amd64.deb`

6. Выполните поиск устройств:\
   `sudo scanimage -L`

7. Убедитесь, что в выводе присутствует имя устройства с упоминанием драйвера **canondr**.

8. Выполните тестовое сканирование через утилиту **fly-scan** "Сканирование".

9. В случае необходимости удаления драйвера выполните команду:\
   `sudo apt purge cndrvsane-drc225`