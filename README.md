# Configuración de i3wm con Polybar en Arch Linux

## Dependencias instaladas para el uso de i3wm

## Para i3wm

#### Por pacman

- pcmanfm - Gestor de archivos
- dmenu - Menú para abrir aplicaciones
- nitrogen - Para cambiar fondo de pantalla
- lxappearance - Cambiar temas e iconos
- picom - Transparencia en ventanas
- rofi - Menú para abrir aplicaciones
- ttf-font-awesome - Fuente para iconos en barra
- i3-lock-color - Bloqueo de pantalla
- xorg-fonts-misc - Fuente utilizada en polybar

### Por yay (AUR)

- xmacro - Leer y conoces los nombres de nuestras teclas
- fim - Ver imagenes por consola
- gthumb - Ver imagenes por GUI
- polybar - Herramienta para perzonalizar la barra de estado
- siji-git
- ttf-unifont

## Para desarrollo

- VsCode
- Sublim Text 3
- Robo3t
- PHP
- MySql
- Apache
- NodeJs

## Algunas configuraciones de i3wm

### Asignar programas a escritorios

Primero debemos de saber el nombre de la clase del programa, en una terminal escribimos **xprop** el cursor cambiara a una cruz (debemos de tener abierto el programa que queremos conocer su clase) y damos click sobre el programa, donde dice **WM_CLASS(STRING)="unnombre"** , _"estaEsLaClase"_ y en el archivo de configuración escribir:

> [for_window [class="nombreClase"] move to workspace $ws2]

### Cambiar fondo de escritorio

Se debe de tener un administrador de archivos como **pcmanfm**, abrimos nitrogen, buscamos la ruta donde estan nuestras imagenes (se puede hacer por consola _nitrogen_ _~/images/_ ). Para que se ejecute cada vez que se inicia en el archivo de configuración de i3 escribimos:

> exec nitrogen --restore

_Para más información de configuraciones, como conexión por **WiFi**, etc realice guías que se encuentran en este mismo repositorio, estas guías se realizaron visitando blogs, documentaciones y/o tutoriales._

## Bibliografía y canales de YouTube

https://i3wm.org/docs/userguide.html
https://wiki.archlinux.org/index.php/I3_(Espa%C3%B1ol)
https://wiki.archlinux.org/index.php/Polybar
https://ermannoferrari.net/polybar-config-file
https://github.com/nicomazz/i3-polybar-config
https://victorhckinthefreeworld.com/2018/09/05/bloquear-la-pantalla-en-i3wm-con-una-captura-pixelada-del-escritorio/
https://askubuntu.com/questions/1262791/multiple-monitors-with-i3-window-manager

**EF - Tech Made Simple**

- https://www.youtube.com/channel/UCX_WM2O-X96URC5n66G-hvw

**Gerry Studios**

- https://www.youtube.com/channel/UC08if0oBaJcpxQQaa7wJZ0g

**Zatiel**

- https://www.youtube.com/user/CallMeZatiel
