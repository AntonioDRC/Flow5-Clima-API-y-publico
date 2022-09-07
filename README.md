# Flow5-Clima-API-y-publico
En este repositorio se realizo la comunicacion de forma local y de forma publica en un localhost y en una ip publica

# Introduccion
En este flow se podra observar en una grafica de forma global los datos de temperatura y de humedad que se estan enviando por medio de API y MQTT

# Material necesario 
1.- Ubuntu 20.04
2.-NodeJS
	2.1.-NPM
	2.1.-NodeRed
	2.1.-Nodo Dashboard
3.-Mosquitto

# Material de referencia
1.- Instalación de Virutal Box y Ubuntu 20.04
2.- Instalación de NodeRed
3.- Introducción a NodeRed
4.- Introducción a Mosquitto

# Material de referencia
En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com que te permitirán realiar las configuraciones necesarias

1.- Instalación de Virutal Box y Ubuntu 20.04
2.- Instalación de NodeRed
3.- Introducción a NodeRed
4.- Introducción a Mosquitto

# Servicios
Para que este ejercicio funcione, necesitas los siguientes servicios

1.- HiveMQ. Es un broker publico y no se necesita cuenta
    OpenWeatherMap. Servicio meteorológico gratuito. Se requiere cuenta,
    pero no se requiere ningun pago.
    
# Instrucciones
Para que este flow funcione, debes cumplir con los siguientes requisitos previos

1.- Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna
    versión LTS. Al momento de creación de este documento, se usó la
    versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para
    hacer uso de NPM
    
2.- Instalación de NodeRed. La instalación se realiza por NPM. Al momento
    de la creación de este contenido, se usó la versión 3.0.2
    
3.- Instalar los nodos node-red-dashboard. Para ello, dirigete a la opcion
    "Manage Palet" de NodeRed y en la pestaña Install busca node-red
    dashboard. Finalmente haz clic en instalar.
   
4.- Instalación de Broker local Mosquitto MQTT.
    
5.- Cuenta en OpenWeatherMap.org. Este es el servidor del cual se
    obtendrán los datos del clima por API
    
6.- API Key valida. Deberás generar una API Key con tu cuenta de
    openweathermaps.org

# Instrucciones de preparación del entorno

Para ejecutar este flow, es necesario lo siguiente:

    1.- Arrancar NodeRed con el comando node-red
    2.- Importar el flow del repositorio.
    3.- Coloca tu API Key personal en la API Call del nodo HTTP Request.
    4.- Actualiza la IP del broker público.
    5.- Hacer clic en el boton Deploy.

# Instrucciones de operación

1.- Para observar el resutlado de este flow, abre un navegador y dirígete  a localhost:1880/ui.
2.- Para activar las gráficas de clima manual, debes enviar por MQTT un mensaje que contenga un JSON con las variables ID, temp y hum.

# Notas

1.- La sección manual de este flow se suscribe al tema codigoIoT/fow5/mqtt en un broker local.

2.- El mensaje mqtt usado para probar este flow es mosquitto_pub -h localhost -t ccodigoIoT/fow5/mqtt -m '{"ID":"Hugo Vargas","temp":18,"hum":78}'
    
3.- Para que la gráfica historica muestre información, deben enviarse al menos 2 puntos.
    
4.- Para actualizar la IP del broker publico, se recomienda el siguiente comando nslookup broker.hivemq.com. Puedes usar el broker publico de tu elección.

5.- Para que multiples graficas sean mostradas en la sección de Histórico Público, es necesario que multiples usuarios se encuentren publicando a la vez.

# Resultados
![WhatsApp Image 2022-09-07 at 9 18 11 AM(1)](https://user-images.githubusercontent.com/111295166/188901695-cdcf8d78-b630-44fe-a460-d9fb78fb0454.jpeg)
sultados
![WhatsApp Image 2022-09-07 at 9 14 26 AM](https://user-images.githubusercontent.com/111295166/188901074-8ddb7f8c-ca92-4f90-8a15-c353362cce2c.jpeg)


# Evidenca
![WhatsApp Image 2022-09-07 at 9 14 28 AM](https://user-images.githubusercontent.com/111295166/188901048-b7d0f706-516c-4b3a-ae7d-9c3ee609ab94.jpeg)
ias![WhatsApp Image 2022-09-07 at 9 14 27 AM](https://user-images.githubusercontent.com/111295166/188901065-1974d051-63e5-45ea-b86b-386faf20dd31.jpeg)


# Creditos
1.- CodigoIoT
2.- Profesor Hugo Escalpedo
