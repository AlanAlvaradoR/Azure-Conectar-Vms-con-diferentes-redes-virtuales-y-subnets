# Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets
Creación de dos máquinas virtuales con una red virtual independiente para cada una con subnets

![Logo de VM](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/VM.jpg)

## Requisitos

- Cuenta de [Azure](https://portal.azure.com/) con suscripción activa
- Computadora con Windows, Linux o MacOs

---------------------------------------------------------

## Pasos

- Se inicia sesión en la página de [Azure](https://portal.azure.com/)

![Inicio Azure](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/inicio%20Azure.PNG)

- Se busca "Grupos de recursos" y se presiona enter

![P9-1](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-1.PNG)

- Presionamos en el botón "crear"

![P9-2](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-2.PNG)

- Le damos un nombre al grupo de recursos y presionamos "revisar y crear"

![P9-3](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-3.PNG)

- Esperamos a que termine la validación y se habilite el botón de "crear". Presionamos el botón "crear"

![P9-4](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-4.PNG)

- El grupo de recursos se va a implmentar casi de manera instantanea. Ahora nos dirigimos al buscador y buscamos "redes virtuales" damos click en la opción indicada en la imagen.

![P9-5](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-5.PNG)

- Damos en el botón de "crear"

![P9-6](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-6.PNG)

- Seleccionamos el grupo de recursos que acabamos de crear, le damos un nombre y seleccionamos de región "Australia Este"

![P9-7](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-7.PNG)

- Después damos click en la pestaña de "direcciones IP"

![P9-8](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-8.PNG)

- En el apartado de subredes marcamos la casilla de la subred "default" y seleccionamos "quitar la subred"

![P9-9](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-9.PNG)

- Después damos click en "agregar subred"

![P9-10](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-10.PNG)

- Se abrirá una pestaña lateral donde debemos colocar el nombre de la subred y en el intervalo de direcciones de subred poneos "10.0.0.0/24" y presionamos "agregar"

![P9-11](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-11.PNG)

- Nos aparecerá la subred que creamos en el apartado de subredes. Presionamos "revisar y crear"

![P9-12](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-12.PNG)

- En la siguiente pestaña esperamos a que se nos habilite la opción de "crear" y después la presionamos

![P9-13](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-13.PNG)

- Esperamos hasta que se logre la implementación y muestre una vantana como la siguiente. 

![P9-14](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-14.PNG)

- Abrimos otra ventana del navegador e ingresaos a [Azure](https://portal.azure.com/)

- En el buscador de la parte superior buscamos "Máquinas virtuales" y seleccionamos la opción que se muestra en la imagen

![P9-15](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-15.PNG)

- Presionamos en "crear" y luego en "Máquina virtual de Azure"

![P9-16](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-16.PNG)

- En el apartado de "grupo de recursos" seleccionamos el grupo de recursos que creamos anteriormente y le damos un nombre a la primera máquina virtual

![P9-17](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-17.PNG)

- Seleccionamos la región "Autralia Este", Imagen "Ubuntu server", el tamaño por defecto y tipo de autenticación "contraseña"

![P9-18](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-18.PNG)

- Creamos un usuario y contraseña

![P9-19](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-19.PNG)

- Subimos en la página y cambiamos a la pestaña "redes"

![P9-20](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-20.PNG)

- Allí seleccionamos la red virtual que acabamos de crear y le damos click a "revisar y crear"

![P9-21](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-21.PNG)

- Esperamos a que se validen las configuraciones y se habilite el botón de "crear". Presionamos "crear"

![P9-22](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-22.PNG)

- Se mostrará una pantalla de carga donde debemos esperar a que se implemente la VM

![P9-23](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-23.PNG)

- Una vez terminada la implementación se mostrará una pantalla como la siguiente:

![P9-24](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-24.PNG)

- Abrimos otra ventana del navegador e ingresaos a [Azure](https://portal.azure.com/)


- Nos dirigimos al buscador y buscamos "redes virtuales" damos click en la opción indicada en la imagen.

![P9-5](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-5.PNG)

- Damos en el botón de "crear"

![P9-6](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-6.PNG)

- Seleccionamos el grupo de recursos que acabamos de crear, le damos un nombre y seleccionamos de región "Australia Este"

![P9-25](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-25.PNG)

- Después damos click en la pestaña de "direcciones IP"

![P9-8](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-8.PNG)

- En el apartado de subredes marcamos la casilla de la subred "default" y seleccionamos "quitar la subred"

![P9-9](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-9.PNG)

- Después damos click en "agregar subred"

![P9-10](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-10.PNG)

- Se abrirá una pestaña lateral donde debemos colocar el nombre de la subred y en el intervalo de direcciones de subred poneos "10.1.0.0/16" y presionamos "agregar"

![P9-26](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-26.PNG)

- Nos aparecerá la subred que creamos en el apartado de subredes. Presionamos "revisar y crear"

![P9-12](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-12.PNG)

- En la siguiente pestaña esperamos a que se nos habilite la opción de "crear" y después la presionamos

![P9-27](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-27.PNG)


- Abrimos otra ventana del navegador e ingresaos a [Azure](https://portal.azure.com/)

- En el buscador de la parte superior buscamos "Máquinas virtuales" y seleccionamos la opción que se muestra en la imagen

![P9-15](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-15.PNG)

- Presionamos en "crear" y luego en "Máquina virtual de Azure"

![P9-16](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-16.PNG)

- En el apartado de "grupo de recursos" seleccionamos el grupo de recursos que creamos anteriormente y le damos un nombre a la primera máquina virtual. Seleccionamos la región "Autralia Este", Imagen "Ubuntu server", el tamaño por defecto y tipo de autenticación "contraseña". Creamos un usuario y contraseña.

![P9-28](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-28.PNG)

- Subimos en la página y cambiamos a la pestaña "redes"

![P9-20](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-20.PNG)

- Allí seleccionamos la red virtual que acabamos de crear y le damos click a "revisar y crear"

![P9-29](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-29.PNG)

- Esperamos a que se validen las configuraciones y se habilite el botón de "crear". Presionamos "crear"

![P9-22](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-22.PNG)

- Se mostrará una pantalla de carga donde debemos esperar a que se implemente la VM

![P9-23](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-23.PNG)

- Una vez terminada la implementación se mostrará una pnatalla como la siguiente:

![P9-30](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-30.PNG)

- Abrimos el Shell de Azure, para ello presionamos el botón superior indicado en la siguiente imagen

![P9-31](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-31.PNG)

- Se abrirá una terminal en la parte inferior con un mensaje como el siguiente

![P9-32](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-32.PNG)

- Si no se ha creado una cuenta de almacenamiento anteriormente, se mostrará el siguiente aviso. Aquí se presiona el botón de "crear almacenamiento"

![P9-33](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-33.PNG)

- Se selecciona PowerShell y la terminal cambiará de color y se verá así

![P9-34](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-34.PNG)

- Una vez termine de cargar, se mostrará lo siguiente

![P9-35](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-35.PNG)

- Ahora volvemos a la página del recurso de la primer máquina virtual que creamos y en el menú lateral izquierdo seleccionamos "conectar"

![P9-36](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-36.PNG)

- Después, en el apartado SSH seleccionamos y copiamos el comando que nos muestre en la siguiente ubicación (único y diferente por usuario)

![P9-37](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-37.PNG)

- Volvemos a la página de la terminal y escribimos "ssh" y después le pegamos el texto que copiamos anteriormente, se vería algo así

``` Bash
ssh AlanAlv@20.53.228.47
```
![P9-38](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-38.PNG)
- Presionamos enter y nos mostrará el siguiente aviso, escribimos "yes" y damos enter

![P9-39](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-39.PNG)

- Escribimos la contraseña de la cuenta que creamos en esa máquina virtual y damos enter (puede que parezca que no estamos escribiendo, pero si lo hacemos)

![P9-40](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-40.PNG)

- Escribimos el siguiente código para verificar si la conexión fue exitosa

``` Bash
sudo apt-get moo
```

- Debe aparecernos algo así

![P9-41](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-41.PNG)

- Después, volvemos a la pestaña con el recurso de la primera red virtual que creamos (con la que conectamos la primer VM) y en el menú lateral izquierdo desplazamos un poco hacia abajo hasta encontrar el apartado "emparejamientos" y damos click

![P9-42](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-42.PNG)

- Nos mostrará la siguiente ventana. Seleccionamos "agregar"

![P9-43](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-43.PNG)

- Colocamos un nombre del vínculo de emparejamiento, y en el nombre del vinculo de la red virtual remota colocamos el mismo nombre la primer pero a la inversa, como se muestra a continuación

![P9-44](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-44.PNG)

- Bajamos sobre la misma página y en el apartado de "red virtual" seleccionamos el nombre de la segunda red virtual que creamos y finalmente presionamos "agregar

![P9-45](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-45.PNG)

- Se mostrará el emparejamiento creado parecido al siguiente

![P9-46](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-46.PNG)

- Presionamos en el botón actualizar cada minuto hasta que en el estado aparezca "conectado"

![P9-47](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-47.PNG)

- Ahora volvemos a la terminal y escribimos el siguiente comando y damos enter

```Bash
ping 10.0.0.4
```
![P9-48](https://github.com/AlanAlvaradoR/Azure-Conectar-Vms-con-diferentes-redes-virtuales-y-subnets/blob/main/imagenes/P9-48.PNG)

- NOTA: en este último paso se debe poner la dirección IP de la segunda VM que creamos que puede consultarse accediendo a la red virtual que creamos -> dispositivos conectados



