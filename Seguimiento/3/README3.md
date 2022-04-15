Punto 1:

1.1 se crearon los dos grupos desde mi usuario con el comando:

sudo groupadd profesores
sudo groupadd estudiantes












Punto 2:

2.1 se crearon los tres respectivos usuarios con el comando:

sudo adduser diana
sudo adduser claudia
sudo adduser laura














Punto 3:

3.1 Se asignaron los usuarios a los grupos de la siguiente forma :

grupo profesores — diana y claudia
grupo estudiantes — laura

esto se hizo con el siguiente comando:

sudo usermod diana -G profesores
sudo usermod claudia -G profesores
sudo usermod Laura -G estudiantes














Nota: se verifico el paso anterior con el comando: cat /etc/group el cual me sirve para ver los grupos y los usuarios pertenecientes a dichos grupos2








3.2 Se crearon los directorios D.Profesores y D.Estudiantes con el comando mkdir en la ubicación /home esto para evitar los problemas con los permisos de cada usuario










3.3 se les asigno el respectivo grupo dueño a los directorios recientemente creados con el comando:

sudo chgrp -R profesores /home/D.Profesores — El grupo profesores es dueño del directorio                       						                                                      D.Profesores


sudo chgrp -R estudiantes /home/D.Estudiantes —  El grupo estudiantes es dueño del directorio                       						                                                         D.Estudiantes 














Punto 4: 

4.1 Se les asigno los respctivos accesos como lo indica el punto con el comando:

sudo chmod 070 /home/D.Profesores  — Da acceco de rwx a grupos

sudo chmod 077 /home/D.Estudiantes — Da acceco de rwx a grupos y otros













Punto 5:

5.1 Se verificaron los permisos anteriormente concedidos entrando a cada usuario con el comando : sudo su nombreUsuario y viendo si este tenia acceso a su o sus respectivos directorios

Usuario diana:















Usuario claudia:
















usuario laura:














Punto 6:

6.1 Entre a los directorios creados con los tres usuarios y con cada uno cree un archivo con el comando vi


Usuario diana:









Usuario Claudia:










Usuario Laura:









Punto 7:

7.1 Cambie el usuario a súper usuario (root) y revise el dueño de los directorios , el resultado es el siguiente :











Después intercambie de dueños a los archivos notasPrimerCorte y notasSegundoCorte con el comando:

chown claudia notasPrimerCorte

chown diana notasSegundoCorte

Quedaría de la siguiente manera: 















Punto 8:

8.1 Usando diferentes terminales entre al sistema con diferentes usuarios equivocándome unas veces por completo en nombre de usuario y contraseña




































Punto 9:

9.1 Usando diferentes terminales accedí al sistema equivocándome algunas veces en el nombre de usuario o contraseña































Punto 10:

10.1 con el comando last liste los ingresos al sistema y pude ver que laura ingreso 2 veces al sistema



































Punto 11:

11.1 con el comando tar cvfz nombreComprimido.tgz D.Profesores comprimi el directorio D.Profesores en un archivo .tgz con el nombre profesore.tgz






















11.2 con el comando  zip -r  nombreComprimido.zip D.Estudiantes comprimi el directorio D.Estudiantes en un archivo .zip con el nombre estudiantes.zip












Punto 12:

12.1 Con el comando alias cc =”sudo paswwd diana”  hicimos un atajo para cambiar la clave del usuario diana al ejercer el atajo cc

















