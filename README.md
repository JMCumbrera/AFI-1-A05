# Adquisición Forense de una memoria USB

Para la realización de esta actividad elegiremos una memoria USB de 8GB de espacio, de marca Kingston Data Traveler.

## AccessData FTK Imager

Comenzamos usando la aplicación FTK Imager en una máquina virtual con Windows 10. Para realizar el clonado de la susodicha memoria USB elegimos la pestaña ***Create Disk Image*** para crear una imagen del pen-drive, elegimos la opción ***Physical Drive*** o "Disco físico" y finalmente elegimos el pen-drive cuando se nos dé la opción.

![FTK3](img/FTK3.png)

El formato que elegiremos para el clonado será el formato en bruto o ***Raw***, y después de esto rellenaremos la información que se nos pide.

![FTK4](img/FTK4.png)

![FTK5](img/FTK5.png)

Antes de comenzar con el clonado del pen-drive deberemos elegir donde depositar el clonado de la memoria USB, además de darle un nombre.

![FTK6](img/FTK6.png)

Luego podremos ver cómo se clona la memoria USB elegida.

![FTK7](img/FTK7.png)

Terminado todo el proceso veremos en el escritorio (lo he elegido paara la demostración) la imagen creada de la memoria USB junto con un extracto en formato txt que contiene los detalles más importantes del clonado y de la memoria USB. Además, también podemos verificar el hash de la memoria clonada, comparándolo con el de la memoria USB que hemos clonado.

![FTK8](img/FTK8.png)

![FTK9](img/FTK9.png)

![FTK10](img/FTK10.png)

<br/>

## GuyImager

Para usar esta herramienta, hemos elegido el SO CAINE, usado para el ámbito de la forensia digital. Lo primero que haremos será elegir nuestro dispositivo USB y elegir la opción ***Acquire Image***, y luego optaremos por una imagen de formato .dd. Finalmente sólo tendremos que elegir una ubicación y darle un nombre a la imagen que adquiriremos.

![GuyMager1](img/GuyMager1.png)

![GuyMager2](img/GuyMager2.png)

![GuyMager3](img/GuyMager3.png)

Cuando termine la operación, podremos acceder a la información generada tanto en la carpeta donde se ha creado la imagen o haciendo clic en la opción ***Info***

![GuyMager4](img/GuyMager4.png)

![GuyMager5](img/GuyMager5.png)

![GuyMager6](img/GuyMager6.png)

Como podemos ver, ya tenemos nuestra imagen forense en formato .dd de la memoria USB original

<br/>

## Comando dd

