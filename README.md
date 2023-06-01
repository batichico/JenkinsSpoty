Ejercicio Integrador
Nos contrataron de la empresa Spotify dentro del area de Sistemas, y somos los encargados de implementar procesos de CI/CD dentro
de la organización. Para ellos, nuestro gerente nos solicito que desarrollemos un proceso integrado, para ello, debemos generar
2 tareas en Jenkins:
1) La tarea debe acceder al repositorio: https://github.com/Ripper2021/CICD_Jenkins y descargar la información de la rama principal
2) La segunda tarea, debe esperar a que la primera finalice, y una vez finalizada debe declarar en un pipeline lo siguiente:
- Si el día es Jueves, debe realizar los siguientes comandos de Maven: clean install
- Si el día es Viernes, debe mover el .jar al disco C: local
- Si el día es Lunes y Martes, no hace nada. 
- Sl el día es Miercoles hacemos pruebas unitarias (mvn test)
(!) 
- SIEMPRE DEBE INFORMAR el usuario que lo ejecuta 
- Debe enviar un mail al usuario en caso de que el pipeline falle
- Debe tener seteado el timeOut en 30 minutos, como opción. 
(!) 

ENTREGABLES: 
- Codigo del pipeline declarativo
- Captura de la tarea que baje la información del repositorio, en el caso que sea de estilo libre. En el caso que lo hagan con un 
pipeline declarativo, el codigo de Groovy.
