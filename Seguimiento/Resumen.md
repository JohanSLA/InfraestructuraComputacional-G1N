como contenerizar una aplicaión java ?

Pasos:
1-Crear el codigo o aplicaión ren java (una herramienta que es de gran ayuda es Spring)

2-Desempaquetar lo que la pagina genera y abrirla con el visualizador de preferencia,importamos Requestmapping
y RestController para etiquetarlos y asi construir un metodo que responda por la URL del api y que este traiga 
un mensaje (con tree se puede visualizar el contenido de todo el proyecto en forma de arbol)

3-Para lo que viene debemos asegurarnos que tenemos instalado el java (En caso de no tenerlo se debe realizar 
dicha descarga e insatalación) , tambien es necesario ver la version del mvn (Esto lo podemos hacer con el comando:
mvn --version) en caso de no aparecer debemos exportarlo.

4-Debemos mirar los objetos con el comando ls -lrt y revisar si tenemos un compilado con el comando target 
(Si esta compilado nos mostrara un archivo con extensión .jar)

5-Entramos al DockerFile el cual nos permite tomar el compilado

6-Procedemos a contruir una imagen con el comandio: docker build -f DockerFile-build -t spring-boot .

7-Debemos ejecutar esta imagen en un contenedor con el comando: docker run -p 8080:8080 -t spring-boot 

Nota:Docker desktop permite ver que se esta haciendo ,ver variables de entorno,entre muchas mas funciones.
En pocas palabras ayuda a administrar nuestros contenedores 

Si ejecutamos localhost:8080 veremos lo que teniamos en la aplicaión ( va a responder desde el contendor)
