Punto 1:

1.1 se crearon los dos grupos desde mi usuario con el comando:

sudo groupadd profesores
sudo groupadd estudiantes

![1 1](https://user-images.githubusercontent.com/101069598/163656218-9f6025d3-bbaf-4be8-8dfa-3fbb8f12d064.png)
![1 2](https://user-images.githubusercontent.com/101069598/163656312-905fdfaf-1e8c-43e0-baa4-70dc8eb596c4.png)


Punto 2:

2.1 se crearon los tres respectivos usuarios con el comando:

sudo adduser diana
 ![2 1](https://user-images.githubusercontent.com/101069598/163656326-be398ff5-65ef-4992-9c1f-ef70c58d94fa.png)


sudo adduser claudia
![2 2](https://user-images.githubusercontent.com/101069598/163656330-558649a6-bbb5-45af-9921-d38bc3295a31.png)


sudo adduser laura
![2 3](https://user-images.githubusercontent.com/101069598/163656336-0176b49d-034d-48cd-8270-3e3e3e66c280.png)



Punto 3:

3.1 Se asignaron los usuarios a los grupos de la siguiente forma :

grupo profesores — diana y claudia
grupo estudiantes — laura

esto se hizo con el siguiente comando:

sudo usermod diana -G profesores
 ![3 1](https://user-images.githubusercontent.com/101069598/163656345-102dd2b0-8e3b-4c38-8ede-c3388e29c04c.png)


sudo usermod claudia -G profesores
 ![3 2](https://user-images.githubusercontent.com/101069598/163656352-5465a20f-388a-41bd-a97e-98af6caf591d.png)


sudo usermod Laura -G estudiantes
 ![3 3](https://user-images.githubusercontent.com/101069598/163656359-a87e5e7d-721b-4dd7-8f52-0df6974ede77.png)



Nota: se verifico el paso anterior con el comando: cat /etc/group el cual me sirve para ver los grupos y los usuarios pertenecientes a dichos grupos2

![3 4](https://user-images.githubusercontent.com/101069598/163656362-5f2c5016-c245-4488-b974-5bbeaff77991.png)




3.2 Se crearon los directorios D.Profesores y D.Estudiantes con el comando mkdir en la ubicación /home esto para evitar los problemas con los permisos de cada usuario

![3 5](https://user-images.githubusercontent.com/101069598/163656369-0cc94ca1-40f8-4b11-b7a7-6709addbf2c5.png)

 ![3 6](https://user-images.githubusercontent.com/101069598/163656378-3d515542-abc0-4565-a5cf-830d8c3c2078.png)



3.3 se les asigno el respectivo grupo dueño a los directorios recientemente creados con el comando:

sudo chgrp -R profesores /home/D.Profesores — El grupo profesores es dueño del directorio                       						                                                                           D.Profesores


sudo chgrp -R estudiantes /home/D.Estudiantes —  El grupo estudiantes es dueño del directorio                       						                                                                          D.Estudiantes 



 ![3 7](https://user-images.githubusercontent.com/101069598/163656400-b990ddf4-aaf8-4d1e-9272-5b876868d9be.png)


![3 8](https://user-images.githubusercontent.com/101069598/163656411-04b04b3f-4731-4b0d-9f2a-232d8d254bd1.png)



Punto 4: 

4.1 Se les asigno los respctivos accesos como lo indica el punto con el comando:

sudo chmod 070 /home/D.Profesores  — Da acceco de rwx a grupos

sudo chmod 077 /home/D.Estudiantes — Da acceco de rwx a grupos y otros

![4 1](https://user-images.githubusercontent.com/101069598/163656422-a60f5eab-450a-48a0-8d5c-5a8213460379.png)

 ![4 2](https://user-images.githubusercontent.com/101069598/163656426-e12730f1-7d1f-499e-872b-ea69f5054466.png)



Punto 5:

5.1 Se verificaron los permisos anteriormente concedidos entrando a cada usuario con el comando : sudo su nombreUsuario y viendo si este tenia acceso a su o sus respectivos directorios

Usuario diana:

 ![5 1](https://user-images.githubusercontent.com/101069598/163656434-4e1e2bac-82e3-4298-80d7-02e8a4ed76df.png)


Usuario claudia:

 ![5 2](https://user-images.githubusercontent.com/101069598/163656437-c69599ff-be9e-4fde-80dd-301e96e8dc64.png)



usuario laura:

![5 3](https://user-images.githubusercontent.com/101069598/163656440-fba68b20-e3b9-4be3-adb0-501320af4ff4.png)




Punto 6:

6.1 Entre a los directorios creados con los tres usuarios y con cada uno cree un archivo con el comando vi


Usuario diana:

![6 1](https://user-images.githubusercontent.com/101069598/163656443-43702e51-9ad9-48eb-ac32-004109518ab5.png)

![6 2](https://user-images.githubusercontent.com/101069598/163656450-a554e83e-6abc-4d3b-ab8d-a41ea811b13a.png)



Usuario Claudia:

 ![6 3](https://user-images.githubusercontent.com/101069598/163656465-5417c61b-b6b5-47e7-9365-8716cd5da717.png)

![6 4](https://user-images.githubusercontent.com/101069598/163656471-ead570c9-58b6-4a71-b21b-eba593de550c.png)



Usuario Laura:

![6 5](https://user-images.githubusercontent.com/101069598/163656482-df6de0ae-0059-456f-ad04-2fb7aa566efa.png)



Punto 7:

7.1 Cambie el usuario a súper usuario (root) y revise el dueño de los directorios , el resultado es el siguiente :

![7 1](https://user-images.githubusercontent.com/101069598/163656493-176b18cf-f54c-4120-a45c-bcd66a4f7f9d.png)


Después intercambie de dueños a los archivos notasPrimerCorte y notasSegundoCorte con el comando:

chown claudia notasPrimerCorte

chown diana notasSegundoCorte

Quedaría de la siguiente manera: 

![7 2](https://user-images.githubusercontent.com/101069598/163656501-2a2ad5dd-a843-4d2a-b6cd-16ee114d5d41.png)



Punto 8:

8.1 Usando diferentes terminales entre al sistema con diferentes usuarios equivocándome unas veces por completo en nombre de usuario y contraseña

![8 1](https://user-images.githubusercontent.com/101069598/163656510-3fef7435-e93d-4fd3-b4b0-1d10da8359a5.png)

![8 2](https://user-images.githubusercontent.com/101069598/163656515-177785d8-ad1f-429b-8ec8-cd450215f39b.png)

![8 3](https://user-images.githubusercontent.com/101069598/163656522-3d1527ad-6bbe-4e90-b0a4-91d5036bae14.png)

![8 4](https://user-images.githubusercontent.com/101069598/163656530-537d6e07-2472-48fc-9a63-960cffbf36de.png)

![8 5](https://user-images.githubusercontent.com/101069598/163656532-ecbacd17-0515-42c5-81ab-b825cab33457.png)



Punto 9:

9.1 Usando diferentes terminales accedí al sistema equivocándome algunas veces en el nombre de usuario o contraseña


![9 1](https://user-images.githubusercontent.com/101069598/163656552-fb9dcb40-d513-4e8f-9d99-c6e7c6360040.png)

![9 2](https://user-images.githubusercontent.com/101069598/163656557-6b512583-7f06-4713-a187-caeed4a05116.png)

![9 3](https://user-images.githubusercontent.com/101069598/163656567-c246ac2f-78ea-4eb6-a1f5-52ddfb5322c1.png)



Punto 10:

10.1 con el comando last liste los ingresos al sistema y pude ver que laura ingreso 2 veces al sistema

![10 1](https://user-images.githubusercontent.com/101069598/163656574-4437711c-ba23-45b4-92fa-60cdbc334af0.png)



Punto 11:

11.1 con el comando tar cvfz nombreComprimido.tgz D.Profesores comprimi el directorio D.Profesores en un archivo .tgz con el nombre profesore.tgz

![11 1](https://user-images.githubusercontent.com/101069598/163656588-529fb05f-c4d2-43b9-9c58-b0773e3995b2.png)

![11 2](https://user-images.githubusercontent.com/101069598/163656594-e6f82d9a-60f0-48d1-b1ae-1676b13346e6.png)



11.2 con el comando  zip -r  nombreComprimido.zip D.Estudiantes comprimi el directorio D.Estudiantes en un archivo .zip con el nombre estudiantes.zip

![11 3](https://user-images.githubusercontent.com/101069598/163656599-db4e6335-15a5-45ac-a400-8e847c3717d8.png)

![11 4](https://user-images.githubusercontent.com/101069598/163656603-5d541372-7f54-4a64-8079-fdc6ff16ffd3.png)



Punto 12:

12.1 Con el comando alias cc =”sudo paswwd diana”  hicimos un atajo para cambiar la clave del usuario diana al ejercer el atajo cc

![12 1](https://user-images.githubusercontent.com/101069598/163656613-fd127ea4-fd28-4d58-ad86-cc4cebcf25cf.png)



