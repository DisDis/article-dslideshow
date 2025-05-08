
Flutter photoframe on Raspberry Pi 4/5 with Human detection, buttons. (Google photo, local storage)

Features:
* Shows a slideshow with different effects.
* Pause/Play
* Screen On/Off
* Support Image/GIF/Video
* Support 2560x1600 resolution
* [Optional] Shows media only when there are people nearby. Fall asleep if there is no movement nearby.
* [Optional/**WIP**] Can download photos/video from Google Photo (non-trivial setting)  
* Over-the-air update (OTA)
* Support MQTT
* Web config [**Work in Progress**]

# Version - v7
[Video](https://youtu.be/eRx7BAgu3N0)
[![Demo](https://img.youtube.com/vi/eRx7BAgu3N0/0.jpg)](https://youtu.be/eRx7BAgu3N0)

# Common view
![3d_1.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/3d_1.png)
![3d_2.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/3d_2.png)
![common_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/common_1.jpg)
![common_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/common_2.jpg)

# — English Text —

 # Motivation
They have worse quality of display, Usually it has 720p, sometimes you can find 2K display. But the most frustration to if you leave room it demonstrates photos to a empty room. And you must power off the photoframe. Therefore, you have to manually turn off such “photoframe”, and therefore then there is no desire to turn them on, since this is an unnecessary action. Most of photoframes need to store media to usb or do a lot of action to upload new photos to a device. Of course there is no integration with smart home.
And at some moment I decided to change this situation. Thus began a 5 year long story...

# Making a photoframe
## What you need for assembly
- Electronic components
  - 1 * RaPi4 (min 1Gb) / RaPi5 + Aluminum Heatsink (min)
  - [Optional] 1 * LED (something like LED Diode 5 mm) 
  - [Optional for LED] 3.3K Ohm resistor
  - [Recommend] 4 * Button (6*6*9 min)
  - [Recommend] PCB_Buttons 
  - [Recommend] 1 * HLK-LD2410 - 24GHz Smart Human Presence Sensing Radar Module ([Ali](https://aliexpress.com/item/1005004786874722.html)) 
  - 1 * 2560*1600 Display (TFTMD089030 + Driver TC358870XBG) ([Ali](https://aliexpress.com/item/1005002008224190.html))
    - **SUPPORTED only** TC358870XBG driver!
    - 197.60(W) x 129.60(H) mm
  -  1 * Power supply 30W min (9-30V) 5.5x2.1 (5.5.x2.5)
  - 1 * Female DC Power plug 5.5х2.1mm DC-099 ([Ali](https://aliexpress.com/item/4000053061172.html))
  - 1 * DC-DC 9-30V -> 5V5A ( [Ali](https://aliexpress.com/item/32763711912.html) )
  - 1 * MicroUSB connector male (for LCD driver)
  - 1 * USB Type-C connector male (for RaPi)
  - 1 * HDMI - Micro-HDMI (30cm max!)
  - 1 * microSDXC for Media 
  - Wires :) (0.75mm2, 0,12mm2, 0,07mm2)
- 1 * Glass - 235x170x2mm (recommend - **233х168х2**, max - 234x169x2, min - 230x165x1.5) 
- Glue-gun
- 2 * M2х8 Countersunk Flat Head Bolt for Body
- 2 * M2х6 Countersunk Flat Head Bolt for PCB_Buttons
- 4 * M2х3.5(3.2) Copper Insert Nut
- 2 * WAGO 3 port 2.5mm2 - Mount connection terminal WAGO 2273-203
- 1.8(1.75)mm, 3.5mm drill 

## What you need to print.
- 1 * Body (Body) with tree-supports
- 1 * Screen holder (Screen Holder = SH)
- 1 * Back cover of the device (Back) with tree-supports.
- 4 * Screen retainers (Screen retainers = SR)
- 1 * Universal PCB_Buttons for buttons “PCB_dslideshow”, [dslideshow - EasyEDA](https://easyeda.com/igor.demyanov/dslideshow) you can order by jlcpcb. 

I recommend printing with ‘Only one wall on top surfaces’ and ‘Only one wall on first layer’. Use a 0.2mm layer.
Use tree-supports, ‘on build plate only’, ‘Support/object first layer gap’ = 0.4mm’ 
![orca_1.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/orca_1.png)
![orca_2.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/orca_2.png)
![orca_3.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/orca_3.png)



 **IN PROGRESS**

 **IN PROGRESS**
 *IN PROGRESS*
 **IN PROGRESS**

 **IN PROGRESS**

# — Original Text —

# Мотивация
На самом деле я не люблю фоторамки. Они отвратительного качества - чаще всего 720p, в редких случаях вы получаете 2К разрешение. Но больше всего расстраивает, что когда ты уходишь, тебе надо отключать её, так как она просто будет показывать фотки в пустоту. Поэтому надо руками отключать такие “рамки”, а следовательно потом нет желания включать, так как это лишнее действие. Большинство рамок требуют записывать данные на usb, или ещё проводить кучу манипуляций для передачи фотографий на устройство. Ну и само собой, нет никакой интеграции с умным домом.
И в какой-то момент я решил исправить эту ситуацию. Так началась история длинною в 5 лет…

# Изготовление
## Что нужно для сборки?
- Electronic components
  - 1 * RaPi4 (min 1Gb) / RaPi5 + Aluminum Heatsink (min)
  - [Optional] 1 * LED (something like LED Diode 5 mm) 
  - [Optional for LED] 3.3K Ohm resistor
  - [Recommend] 4 * Button (6*6*9 min)
  - [Recommend] PCB_Buttons 
  - [Recommend] 1 * HLK-LD2410 - 24GHz Smart Human Presence Sensing Radar Module ([Ali](https://aliexpress.com/item/1005004786874722.html)) 
  - 1 * 2560*1600 Display (TFTMD089030 + Driver TC358870XBG) ([Ali](https://aliexpress.com/item/1005002008224190.html))
    - **SUPPORTED only** TC358870XBG driver!
    - 197.60(W) x 129.60(H) mm
  -  1 * Power supply 30W min (9-30V) 5.5x2.1 (5.5.x2.5)
  - 1 * Female DC Power plug 5.5х2.1mm DC-099 ([Ali](https://aliexpress.com/item/4000053061172.html))
  - 1 * DC-DC 9-30V -> 5V5A ( [Ali](https://aliexpress.com/item/32763711912.html) )
  - 1 * MicroUSB connector male (for LCD driver)
  - 1 * USB Type-C connector male (for RaPi)
  - 1 * HDMI - Micro-HDMI (30cm max!)
  - 1 * microSDXC for Media 
  - Wires :) (0.75mm2, 0,12mm2, 0,07mm2)
- 1 * Glass - 235x170x2mm (recommend - **233х168х2**, max - 234x169x2, min - 230x165x1.5) 
- Glue-gun
- 2 * M2х8 Countersunk Flat Head Bolt for Body
- 2 * M2х6 Countersunk Flat Head Bolt for PCB_Buttons
- 4 * M2х3.5(3.2) Copper Insert Nut
- 2 * WAGO 3 port 2.5mm2 - Mount connection terminal WAGO 2273-203
- 1.8(1.75)mm, 3.5mm drill 

## Что нужно напечатать\заказать.
- 1 * Корпус (Body) с древовидными поддержками
- 1 * Держатель экрана (Screen Holder = SH)
- 1 * Заднюю крышку (Back) + с древовидными поддержками.
- 4 * Фиксаторы экрана (Screen retainers = SR)
- 1 * универсальную плату для кнопок PCB_Buttons  “PCB_dslideshow”, [dslideshow - EasyEDA](https://easyeda.com/igor.demyanov/dslideshow) можно заказать через jlcpcb. 

Рекомендую печатать с опциями 1 периметр на первом и верхних поверхностях (‘Only one wall on top surfaces’, ‘Only one wall on first layer’), высота слоя 0.2мм.
Древовидные поддержки от стола и отступ от модели 0.4мм (‘on build plate only’, ‘Support/object first layer gap’ = 0.4mm’).
![orca_1.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/orca_1.png)
![orca_2.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/orca_2.png)
![orca_3.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/orca_3.png)

## Настройка RaPi4/5
### Установить OS
Скачиваем образ "Raspberry Pi OS Lite (64bit)"
Запускаем rpi-imager добавляем туда 2024-11-19-raspios-bookworm-arm64-lite.img.xz,
Изменяем настройки установки:
- Имя хоста. Например dslideshow1
- SSH - установите доступ по паролю или через ключ (если он у вас есть)
- WiFi (укажите рабочий!)
- user/password (pi/123456)

**Включайте оборудование.**

Ждите пока система не появиться в сети. Обычно на это требуется 1-2 минуты.
Заходим по ssh и ставим все обновления.
>ssh pi@dslideshow1.local

>sudo apt-get update
>sudo apt-get upgrade

Если нужно включить вход ssh через пароль, редактируем строчку в файле */etc/ssh/sshd_config*
>sudo nano /etc/ssh/sshd_config

>PasswordAuthentication yes

### Настройка
Сконфигурируйте /boot/firmware/config.txt
>\# disable sound
>
>dtparam=audio=off
>
>\# disable boost
>
>arm_boost=0
>
>\# UART on
>
>enable_uart=1
>
>\# Bluetooth off
>
>dtoverlay=disable-bt
>
>\# disable splash
>
>disable_splash=1

#### Отключить сервисы связанные с блютус, UART, serial0
>sudo systemctl disable hciuart.service
sudo systemctl disable bluealsa.service
sudo systemctl disable bluetooth.service
sudo systemctl stop serial-getty@ttyS0.service
sudo systemctl disable serial-getty@ttyS0.service

#### Настройка экрана для RaPi4
>sudo nano /boot/firmware/cmdline.txt

Добавить в конце первой строчки:

>“ video=HDMI-A-1:2560x1600M@49 ”

Если что можете проверить какие ваш дисплей поддерживает параметры через 
>edid-decode /sys/class/drm/card1-HDMI-A-1/edid

,а также посмотреть всё ли работает корректно.
>kmsprint -p

#### Отключить serial0
отредактируйте файл
>sudo nano /boot/firmware/cmdline.txt

удалите данный текст 
>“console=serial0,115200 “

#### Настройка разрешений и прав
>sudo usermod -a -G render \$USER
>sudo usermod -a -G dialout \$USER
>sudo usermod -a -G tty \$USER

#### Настройка автоматической Wi-Fi AP (Access Point) 
Source: https://www.raspberryconnect.com/projects/65-raspberrypi-hotspot-accesspoints/203-automated-switching-accesspoint-wifi-network 

Скачайте архив
>curl "https://www.raspberryconnect.com/images/scripts/AccessPopup.tar.gz" -o AccessPopup.tar.gz

Распакуйте
>tar -xvf ./AccessPopup.tar.gz

Перейдите в папку
>cd AccessPopup

Запустите скрипт настройки
>sudo ./installconfig.sh

Выберите вначале.
>1 = Install AccessPopup Script

Далее 

>2 = Change the Access Points SSID or Password

Если не выбрать то: The access points wifi name (ssid) is AccessPopup and the password is 1234567890.

Установите SSID:
>RPiHotspot

Пароль:
>1234567890

#### Установка нужных пакетов.
обновим все пакеты системы.
>sudo apt update
sudo apt upgrade

установим зависимости для работы приложения
>sudo apt install cmake libgl1-mesa-dev libgles2-mesa-dev libegl1-mesa-dev libdrm-dev libgbm-dev ttf-mscorefonts-installer fontconfig libsystemd-dev libinput-dev libudev-dev  libxkbcommon-dev

установим зависимости для видео
>sudo apt install libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libgstreamer-plugins-bad1.0-dev gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad gstreamer1.0-libav gstreamer1.0-alsa

#### Установка DSlideshow
Скачайте последнюю версию [dslideshow-7.x.x-arm64-pi4.deb](https://github.com/DisDis/dslideshow/releases)
залейте её в корень домашней папки 
>/home/pi/

Создайте в корне папку 
>dslideshow

создайте пустой файл 
>config.json

создайте папку 
>images

поместите пару картинок или видео mp4 в папку images.

Установите пакет.
>sudo apt install ./dslideshow-7.2.0+1-arm64-pi4.deb

**Система готова к работе.**

## Подготовка RaPi
- Если вы используете RaPi5 желательно приобрести активное охлаждение, желательно медное - оно тоньше.
- Если вы используете RaPi4 то надо установить радиаторы на горячие чипы.
  - А также удалить выступающие контакты в области Usb3/2 и Eth. Это нужно чтобы всё влезло в корпус, см картинки ![cut_rapi4.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/cut_rapi4.jpg).

## Сборка
### Провода
* От HLK-LD2410 - до RaPi 400mm -0,07мм2 * 3 шт(+,-,Out)
* От PCB_Buttons - до RaPi 270mm - 0,12мм2 * 5 шт (B1,...,Common)

* От DC-099 - до Power pcb - 150mm - 0,75мм2 - 2 шт (+,-)
* От DC-099 - до Wago(p) - 120mm - 0,75мм2 - 1 шт (-)

* От Wago(p) - до Power pcb - 120mm - 0,75мм2 - 1шт (+5v)
* От Wago(p) - до RaPi - 220mm - 0,75мм2(0,5mm2 - min) - 2шт (+,-)
* От Wago(p) - до LCD Driver 300mm - 0,75мм2(0,5mm2 - min) - 2шт (+,-)

* HDMI - MicroHDMI - 300mm(30cm)

* Отрежте филамент(1.75мм) - 22mm - 9шт

### Плата с кнопками и сенсор присутствия людей
**Подготовьте плату с кнопками**. Впаяйте в плату провода(0.12мм2) нужной длины. Припаяйте перемычку(просто кусочек провода) на плату в позицию R5. Припаяйте кнопки к плате. Каждый провод промаркируйте.(B1,B2,B3,B4,Com). Желательно все провода выходящие с платы залить небольшим кол-вом термоклея. К концам провода припаяйте коннекторы для присоединения к 40-pin GPIO header RaPi. 
![button_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_1.jpg)
![button_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_2.jpg)
![button_3.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_3.jpg)
![button_4.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_4.jpg)
![button_5.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_5.jpg)
![button_6.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_6.jpg)
![button_7.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/button_7.jpg)

**Подготовьте радар**(сенсор присутствия людей HLK-LD2410), припаяйте к нему 3 или 5 проводов(0.07мм2) нужной длины. Каждый провод промаркируйте(+5v,R,T,GND,Out). Желательно все провода выходящие с платы залить небольшим кол-вом термоклея. Провода R и T опциональные и нужны если вы хотите перенастраивать чувствительность сенсора в будущем.
К концам провода припаяйте коннекторы для присоединения к 40-pin GPIO header RaPi. 
![human_s_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/human_s_1.jpg)
Я рекомендую припаивать провода прямо к выводам, так как при выпаивании выводов можно повредить плату.(На фото слева)
![human_s_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/human_s_2.jpg)
![human_s_3.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/human_s_3.jpg)
![human_s_4.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/human_s_4.jpg)

### Корпус
Впаяйте в корпус 4 медные вставки М2.
![body_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/body_1.jpg)
![body_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/body_2.jpg)
Проверьте, что медные вставки не выпирают в креплениях кнопок.
![body_3.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/body_3.jpg)
Проверьте, что плата с кнопками подходит.
![body_4.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/body_4.jpg)
Если кнопки заедают и плохо нажимаются, возьмите сверло на 3.5мм и подкорректируйте отверстия для кнопок.
![body_5.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/body_5.jpg)

**Подготовьте держатель экрана(SH)** и **4 фиксатора экрана(SR)**, с помощью сверла 1.8мм, пройдитесь по всем 10 отверстиям SH, и по 8 отверстиям(SR), ваша задача чтобы филамент достаточно плотно заходил в них и не выпадал! 
![sh_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/sh_1.jpg)

Возьмите держатель экрана(SH), установите радар (HLK-LD2410) в нужное место и зафиксируйте клеевым пистолетом, а также прихватите клеем и провода выходящие из радара. Проложите провода через специальный держатель и зафиксируйте его филаментом.
![sh_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/sh_2.jpg)

**Установите экран** в держатель(SH), предварительно удалив защитную плёнку с экрана.
Зафиксируйте экран с помощью 4-х фиксаторов(SR) и нитей филамента, обратите внимание что фиксаторы имеют верх и низ, вверху есть ключ. У фиксаторов слева сделайте филамент подлиннее до края SH или даже может чуть больше(0.5мм), это нужно для фиксации проводов.
![sh_3.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/sh_3.jpg)

Проверьте что задняя крышка входит в пазы в корпусе, при необходимости уберите лишний пластик.

Установить стекло в корпус. (рекомендую выбрать специальное музейное стекло или специально стекло для картинных галерей). Обязательно удалите пыль и всякие загрязнения с внутренней стороны, используйте микрофибру.

Поместите держатель экрана(SH) с экраном на стекло. Проверьте что нет грязи, если есть удалите.
![sh_4.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/sh_4.jpg)

*Временно прикройте белую сторону экрана* толстым картоном или бумагой от клея. Зафиксировать всё клеевым пистолетом, по 4-ём углам держателя экрана(SH), так чтобы держатель экрана не выпадал из корпуса и не двигался внутри. **Будьте осторожны**, нельзя чтобы горячий клей попал на поверхность экрана, это приводит к **выгоранию подсветки экрана**!

Установите плату с кнопками (PCB_Buttons) с помощью 2х  M2 винтов.
Провода проложите под филаментом SR с левой стороны.
Подсоедините все провода к RaPi.
схема подключения: [dslideshow - EasyEDA](https://easyeda.com/igor.demyanov/dslideshow)
- 4 - Buttons 
  - (B1)Back - 16 (23 GPIO)
  - (B2)Menu - 15 (22 GPIO)
  - (B3)ScreenToggle -13 (27 GPIO)
  - (B4)Pause - 11 (17 GPIO)
  - Common - 14 (GND) 
- 1 - HLK-LD2410 pins: 2(+5v), 8(R->TXD0 - 14 GPIO), 10(T->RXD0 - 15 GPIO), 6(GND), 32 (Out - 12 GPIO)

![Schematic_dslideshow_2025-05-03.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/Schematic_dslideshow_2025-05-03.png)

Смотри картинку для подключения, пины для RaPi4/5 можно посмотреть тут: https://pinout.xyz/pinout/wiringpi 

**Проверьте что все +5v, GND, Common** подсоединены к нужным пинам. Все другие пины не подсоединены к +3.3,+5, GND, это важно!

**Установите все три платы в заднюю крышку (back)**. Согните шлейф от драйвера к дисплею как показано на картинке, поместите его в специальное место на задней крышке.

Зафиксируйте клеевым пистолетом все платы. Нанесите клей на каждый пластиковый штырёк и проведите клеем до основания задней крышки, для лучшей фиксации.
![back_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/back_1.jpg)

**Спаяйте usb-mini, usb-c провода нужной длинны**. Обратите внимание на полярность, скачайте заранее спецификацию для ваших плат USB-C
![USB_mini_1.png](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/USB_mini_1.png)
![USB_mini_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/USB_mini_2.jpg)
![USB_C_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/USB_C_2.jpg)

Соедините по схеме.
![wires_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/wires_1.jpg)

Соедините RaPi и драйвер дисплея 30см кабелем HDMI-microHDMI, как показано на картинке.
![wires_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/wires_2.jpg)

**Подготовьте порт питания DC099**. Припаяйте 2 провода на (-) и 1 провод на (+). Центральный пин это (+).
![DC_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/DC_1.jpg)
![DC_2.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/DC_2.jpg)
![DC_3.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/DC_3.jpg)

**Вставьте порт питания DC099 в корпус**, зафиксируйте его в корпусе.
Присоедините длинные провода(+,-) от DC099 к Power_PCB. Короткий провод (-) подключите к WAGO(-) (3pin, 2.5mm2).
![DC_4.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/DC_4.jpg)

Перед окончательной сборкой нужно проверить что все компоненты работают, **проверьте что все (+) и (-) корректно соединены**. Для верности проверьте выходы на Usb-c и usb-mini, это можно сделать через USB тестер или через мультиметр.

Соедините шлейф и экран.
![screen_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/screen_1.jpg)

Итоговая сборка должна выглядеть так:
![final_1.jpg](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/v7/final_1.jpg)

Проверьте что все USB кабели вставлены, все клеммы затянуты, HDMI вставлен до конца. HDMI кабель воткнут в HDMI-0 на RaPi.

Включите систему. Проверьте что всё работает. 
Выключите систему, через меню рамки или через ssh
> sudo shutdown -P now

Выключите питание. Вставьте заднюю крышку в пазы в корпусе, закрутите 2 винта М2.

**Сборка завершена.**

# Как заливать контент
Через SSH\SFTP.
Заливайте в папку **/home/pi/dslideshow/images/**

# Как обновлять
Система поддерживает OTA, по умолчанию рамка включает OTA на 1 минуту после старта.
- Перезагружаете фоторамку.
- Заходите по URL: 
   - >http://dslideshow1.local:8282/ota_start

- Как только вы перейдёте на страницу, рамка переключится в режим загрузки новой версии прошивки, на экране будут показаны код-цифры.
- Введите код с фоторамки в нужное поле
- Прикрепите файл с новой прошивкой
- Нажмите на кнопку upload и рамка загрузит новую прошивку и сама себя обновит.



# History

## Prototype 2
![Proto2_1](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/prototype1/proto2_1.jpg)
![Proto2_2](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/prototype1/proto2_2.jpg)
![Proto2_3](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/prototype1/proto2_3.jpg)
![Proto2_4](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/prototype1/proto2_4.jpg)


Video: [![Demo prototype](https://img.youtube.com/vi/NFGFnHmX0TY/0.jpg)](https://youtu.be/NFGFnHmX0TY)


Backcover prototype:

![Backcover](https://raw.githubusercontent.com/DisDis/article-dslideshow/master/images/prototype1/animation.gif)



https://easyeda.com/igor.demyanov/dslideshow
