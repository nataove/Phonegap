# Taller Phonegap

## Integrantes

* Natalia Rubiano 
* Danny Alexander Carrillo
* Juan Camilo Osorio 


## Características 
### Contactos
La aplicación genera una tabla listando los nombres de los contactos guardados en el celular, la visualización de los números de estos contactos no se genera de forma correcta en dispositivos sin acceso root, por tanto, no se incluyó esta función, sólo se listan los nombres.
Si su dispositivo tiene acceso root, modificar línea 107 del archivo `www/contactos.html`. Agregar:

```javascript
cell2.innerHTML = contacts[i].phoneNumbers[0].value;
```
### Conexión
La aplicación reconoce el tipo de conexión actual y lo muestra en un div. 
Tipos de conexión:

* Conexión desconocida            
* Conexión Ethernet
* Conexión WIFI
* Conexión 2G
* Conexión 3G
* Conexión 4G
* Conexión genérica
* No hay conexión

### Servicio
La aplicación se conecta a:  https://www.datos.gov.co/resource/wcz7-chab.json para leer los sitios turísticos de Tuluá y listarlos en una tabla, se puede acceder al sitio oficial de cada lugar desde la tabla generada. Al generar el .APK esta sección dejó de funcionar. 

### Navegación
Desde los divs de la sección Home se puede acceder a las secciones contactos, conexión y servicio. Además, se cuenta con una barra de navegación que provee la misma funcionalidad. 

### Geolocalización
Se hace uso de la API de Google Maps para mostrar la ubicación actual con una etiqueta, al generar el .APK esta sección dejó de funcionar. 