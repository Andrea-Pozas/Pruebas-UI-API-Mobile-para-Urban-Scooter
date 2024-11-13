# Pruebas-UI-API-Mobile-para-Urban-Scooter
Urban Scooter es una aplicación de renta de Scooter. La aplicación cuenta con versión web desde la cual el usuario puede realizar la renta del Scooter. Así mismo, Urban Scooter cuenta con una aplicación móvil para sus repartidores puedan dar seguimiento a los pedidos y entregas. 
# Herramientas
![Static Badge](https://img.shields.io/badge/Excel-black?style=for-the-badge&logoColor=white&color=%233CB371) ![Static Badge](https://img.shields.io/badge/Jira-%230052CC?style=for-the-badge) ![Static Badge](https://img.shields.io/badge/Android%20Studio-%20%233DDC84?style=for-the-badge&logo=androidstudio&logoColor=black) ![Static Badge](https://img.shields.io/badge/Postman-%23FF6C37?style=for-the-badge) ![Static Badge](https://img.shields.io/badge/C%C3%B3digos%20HTTP-%2373DC8C?style=for-the-badge) ![Static Badge](https://img.shields.io/badge/ApiDoc-%230055DA?style=for-the-badge) ![Static Badge](https://img.shields.io/badge/Figma-%23F24E1E?style=for-the-badge) ![Static Badge](https://img.shields.io/badge/DevTools-black?style=for-the-badge) ![Static Badge](https://img.shields.io/badge/postgresql-%20%234169E1?style=for-the-badge&logo=postgresql&logoColor=black)
# Pruebas para el proceso de renta de un Scooter 
Se realizó una lista de comprobación sobre la pantalla del pedido y pruebas de validación de los datos que se deben ingresar para llenar el formulario de pedido, ambas basadas en los requerimientos y en los diseños contenidos en Figma. Las pruebas incluyen la pantalla estado del pedido y sus etapas.
## Validación de datos del formulario de pedido 
El formulario de pedido pide ingresar al usuario los siguientes datos: nombre, apellido, dirección, estación del metro, teléfono, fecha de entrega, periodo de alquiler, color y comentario. Se realizaron pruebas positivas y negativas tomando en cuenta los valores límites de cada clase para cada campo. 
__ Si quieres ver las pruebas da clic aquí__
## Lista de comprobación de pantalla estado del pedido 
La pantalla de estado del pedido permite al usuario llevar un seguimiento del proceso de renta de su scooter.  El proceso de pedido puede mostrar cinco estados diferentes: El Scooter está en el almacén, el repartidor está en camino, el servicio de entrega llego, pedido atrasado y cancelación del pedido.  Se realizaron pruebas de diseño y funcionales para garantizar que el usuario puede realizar un pedido exitosamente. 
:arrow_right: __Si deseas ver la lista de comprobación da clic aquí__ [Lista de comprobación](https://docs.google.com/spreadsheets/d/19LUq18gnv7S-I8U7Kx7O0LzE4Vb2zwVm/edit?gid=925489201#gid=925489201)
## Resultados 
__Validación de datos del formulario de pedido__ Las pruebas realizadas fueron de utilidad parar encontrar fallas en la admisión de datos, los campos apellido, dirección y teléfono tienen problemas con la longitud de caracteres que se pueden ingresar, el usuario puede agregar más caracteres de los establecidos como límites. En el campo fecha de entrega permite que el usuario elija una fecha pasada 

:arrow_right:__Si deseas ver las pruebas validar los datos de ingreso al formulario da clic aquí__ [Validación de datos](https://docs.google.com/spreadsheets/d/19LUq18gnv7S-I8U7Kx7O0LzE4Vb2zwVm/edit?gid=1773528289#gid=1773528289)

__Pantalla estado de pedido__  Las pruebas funcionales sirvieron para detectar 3 problemas de prioridad alta :
-	 Si el usuario llena el formulario de pedido con datos validos es imposible pedir un Scooter desde la interfaz de Urban Scooter, la página no lo permite. 
-	 Una vez que sea realiza un pedido de un scooter la interfaz no pasa de la etapa 2 de estado de pedido (El repartidor está en camino), a pesar de que el repartidor entregue el scooter nunca cambia y no se marca la fecha de entrega de la renta del scooter 
-	No se puede cancelar un pedido de scooter 
El usuario aún no debería interactuar con Urban Scooter, la aplicación web no está lista para llevar exitosamente el proceso de renta de un scooter. El usuario estaría inconforme al darse cuenta de que no puede alquilar un scooter, visualizar el estado de su pedido ni cancelar su pedido si así lo desea.
 # Pruebas móvil para Urban Scooter 
Urban Scooter cuenta con una aplicación móvil para sus repartidores de scooter. La aplicación permite que el repartidor pueda crear una cuenta y seleccionar de una lista de pedidos del usuario los que desea entregar. Si un repartidor acepta un pedido la aplicación móvil llevará el seguimiento de entrega y notificará al repartidor el tiempo restante para cumplir con la tarea. 
## Casos de prueba para la notificación 
Cuando el repartidor acepta un pedido tiene tiempo límite para entregar el scooter.  Cuando quedan 2 horas para la finalización del tiempo aparece una notificación. Los casos prueba fueron creados y ejecutados para garantizar que la notificación aparece correctamente al repartidor tomando en cuenta el límite de entrega. 
