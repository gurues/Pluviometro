# PLUVIOMETRO DOMÓTICO

## DESCRIPCIÓN DEL PROYECTO

### Este proyecto domótiza un pluviómetro de una estación meteorológica estándar mediante un sensor de puerta zigbee (también se puede usar uno WIFI). El pluviómetro estándar manda una señal de pulso cada vez que registra 0.3 mm de agua de lluvia. Mediante el sensor de puerta registramos estos pulsos que son tratados con NodeRed y Home Assistant para realizar pluviómetro dómotico

![Pluviometro](AYUDA/FOTOS/pluviometro%20(8).jpg)

Para realizarlo son necesarios estos componentes:

* 1 x  [Sensor de puerta Zigbee](https://es.aliexpress.com/item/1005006317651003.html?spm=a2g0o.productlist.main.3.403428d40HaqA6&algo_pvid=283666a9-4e5d-4827-8f7f-751ddbb7c145&algo_exp_id=283666a9-4e5d-4827-8f7f-751ddbb7c145-1&pdp_npi=4%40dis%21EUR%215.92%215.92%21%21%216.46%216.46%21%40211b629217276189974294916e1ec5%2112000036738104594%21sea%21ES%21889791699%21X&curPageLogUid=GoZdAQ3WEirw&utparam-url=scene%3Asearch%7Cquery_from%3A#nav-description) ~ 6€
* 1 x [Pluviómetro Estándar](https://es.aliexpress.com/item/2026877912.html?spm=a2g0o.order_list.order_list_main.321.2efe194dXe8slW&gatewayAdapt=glo2esp) ~ 17€
* Impresión en 3D de soportes y accesorios.

Coste total aproximado 25 euros.

## REALIZACIÓN

Para poder realizar el Pluviómetro debemos realizar los siguientes pasos:

* Desoldad el sensor magnético del sensor de puerta Zigbee.
* Desoldar el sensor magnético del pluviómetro estándar.
* Soldar el sensor magnético del sensor de puerta Zigbee en la posición del sensor magnético del pluviómetro estándar.
* Cortar el cable del pluviómetro estándar a la medida deseada y soldar cada punta al sensor de puerta Zigbee.
* En mi caso instale un nuevo imán de neodimio para mejorar la detección, pero con el que trae puede funcionar.
* Crear el sensor de lluvia en Nodered mediante la importación del archivo sensor_lluvia.json.
* Crear o añadir los utility meter del archivo utility_meter.yaml, para realizar un seguimiento de la precipitación horaria, diaria, semanal, mensual y anual.

## AYUDA

En la carpeta AYUDA se dispone:

* Fotos para ver el resultado final del proyecto.
* Diseño 3D de la caja del dispositivo.
  
## Realizado por gurues (gurues@3DO ~ SEPTIEMBRE 2024 ~ <ogurues@gmail.com>)
