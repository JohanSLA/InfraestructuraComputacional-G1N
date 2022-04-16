Cambio de contraseña para el ususario root
--
1-Se oprimio una tecla para interrumpir el arranque en el grub
2-se presiono la tecla e 
3-se cambio la sentencia rhgb por rd.break 
4-Presionamos las teclas ctrl + x 
5-Presionamos la tecla enter 
6-usamos el comando mount 
7-usamos el comando mount -o rw,remount /sysroot/ 
8-usamos el comando mount 
9-usamos el comando chroot /sysroot/ 
10-usamos el comando passwd, escribimos la contraseña nueva y la rectificamos
12-usamos el comando touch /.autorelabel
13-usamos el comando exit dos veces


Parte 2 (Practica comandos mv y mkdir)
--

1-creamos los directorios Bisabuelo y Bisabuela y dentro de ellos creamos los archivos vi que contienen su informacion
![Captura de pantalla de 2022-04-15 20-54-03](https://user-images.githubusercontent.com/101069598/163657216-5f2f2645-f6f0-4722-b8dd-94d0230ab598.png)
![Captura de pantalla de 2022-04-15 20-54-47](https://user-images.githubusercontent.com/101069598/163657236-9637ac94-e966-44e2-b721-dce3914e54a8.png)
![Captura de pantalla de 2022-04-15 20-55-23](https://user-images.githubusercontent.com/101069598/163657249-84a43efc-d9b2-46c3-a98a-5f771d6f8d08.png)


2-con el comando mv movemos el directorio Abuelo al directorio Bisabuelo
![Captura de pantalla de 2022-04-15 20-58-20](https://user-images.githubusercontent.com/101069598/163657308-0a19161e-3cdf-440d-a280-f5173c0060b3.png)


3-con el comando mv movemos el directorio Abuela al directorio Bisabuela
![Captura de pantalla de 2022-04-15 20-58-58](https://user-images.githubusercontent.com/101069598/163657320-25cd339e-7476-44ee-9304-b583b638592d.png)


4-con el comando mv movemos los archivos de texto del genero masculino a los directorios del genero femenino y viceversa
![Captura de pantalla de 2022-04-15 21-00-48](https://user-images.githubusercontent.com/101069598/163657361-eae9c5a2-b021-4afc-8aba-f94056d439c1.png)
![Captura de pantalla de 2022-04-15 21-02-52](https://user-images.githubusercontent.com/101069598/163657433-23e94d67-fd20-4f3a-8434-fec82e1b1e31.png)
![Captura de pantalla de 2022-04-15 21-04-22](https://user-images.githubusercontent.com/101069598/163657462-305f8336-1606-449d-95be-8c0ad968c245.png)
![Captura de pantalla de 2022-04-15 21-05-28](https://user-images.githubusercontent.com/101069598/163657487-e014cf63-3930-4869-8865-68fb4011c43f.png)

![Captura de pantalla de 2022-04-15 21-11-15](https://user-images.githubusercontent.com/101069598/163657648-6347d5b7-5a98-4bb1-be9b-e901bc8686ff.png)
![Captura de pantalla de 2022-04-15 21-12-43](https://user-images.githubusercontent.com/101069598/163657686-458311a2-3612-4c75-8d15-9cfcae83f546.png)
![Captura de pantalla de 2022-04-15 21-13-50](https://user-images.githubusercontent.com/101069598/163657717-57e39e57-99e0-4ab3-bdde-1dcf78d4b460.png)
![Captura de pantalla de 2022-04-15 21-15-13](https://user-images.githubusercontent.com/101069598/163657747-d6a101d8-f8e1-4c4a-a542-78ac925a07d8.png)


5-creamos los directorios Bisnieta y Bisnieto y a cada uno le creamos sus archivos de texto con su respectiva informacion
![Captura de pantalla de 2022-04-15 21-17-41](https://user-images.githubusercontent.com/101069598/163657797-f0e0801c-38e5-4317-a188-eb476193e4bc.png)
![Captura de pantalla de 2022-04-15 21-18-39](https://user-images.githubusercontent.com/101069598/163657822-8fedd815-5d9b-41ec-8540-6fda6e9aaa0f.png)


6-intercambiamos los archivos de Bisnieta y Bisnieto
![Captura de pantalla de 2022-04-15 21-07-26](https://user-images.githubusercontent.com/101069598/163657589-4f5cd30f-a64f-4aec-877b-354e6ea23055.png)
![Captura de pantalla de 2022-04-15 21-16-48](https://user-images.githubusercontent.com/101069598/163657775-a4a36260-22b2-4ab9-b70b-62667b393067.png)

