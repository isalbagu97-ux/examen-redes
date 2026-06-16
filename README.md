# examen-redes
## Primero instalamos bind9 bind9-utils dnsutils -y
## Configuramos la red con ip fija en mi caso 192.168.10 para el servidor principal la 11 para el secundario
## Y continuamos editando el /etc/bind/named.conf.local
<img width="811" height="522" alt="image" src="https://github.com/user-attachments/assets/715e786c-577e-4ee9-b1fb-daf71453977e" />
## procedemos con los db.agustin.local y su inversa
<img width="738" height="306" alt="image" src="https://github.com/user-attachments/assets/84e8a97b-f616-4792-bf77-76cf927c5971" />

<img width="736" height="349" alt="image" src="https://github.com/user-attachments/assets/21a39c1a-3ce6-4d80-a3b9-ba4b86a50613" />


#Comprobaciones nslookup tanto primario como secundario
<img width="629" height="111" alt="image" src="https://github.com/user-attachments/assets/ed0af4f6-0f4d-4376-ae63-0b35818ad2b6" />

##Esclavo
<img width="729" height="386" alt="image" src="https://github.com/user-attachments/assets/787cd0e0-35e5-422a-9eff-10839e741b9d" />

##Pruebas desde el esclavo

<img width="698" height="150" alt="image" src="https://github.com/user-attachments/assets/dded1b03-1b4d-45fd-90fa-5d037707624b" />

##Añadimos uno nuevo para ver que se crea bien
<img width="741" height="209" alt="image" src="https://github.com/user-attachments/assets/20dbe77f-0868-4e14-b1a3-7ddb631d339b" />
<img width="735" height="208" alt="image" src="https://github.com/user-attachments/assets/0ac24e14-ef7a-4d34-9e1f-8e43d9078a98" />

#PARTE HTTP
## Primero instalamos nginx y configuramos teniendo en cuenta siempre sus ip's
##comprobamos que el cliente pueda entrar en web1 y en web2 despues de las configuraciones
<img width="751" height="87" alt="image" src="https://github.com/user-attachments/assets/96755db7-3c6d-47c7-ba3d-958adedad51a" />
<img width="742" height="101" alt="image" src="https://github.com/user-attachments/assets/5f36801a-c337-496e-9a42-62039a41afd7" />
## .conf de las webs
<img width="734" height="485" alt="image" src="https://github.com/user-attachments/assets/3024267d-5fc3-45fd-ad06-7f23c4f31d63" />
<img width="725" height="477" alt="image" src="https://github.com/user-attachments/assets/0ceafa49-4514-4947-a7d0-0fa854fd4528" />
## comprobaciones de las paginas
<img width="732" height="159" alt="image" src="https://github.com/user-attachments/assets/2a73c4a5-8c6f-449b-8d4f-677c36213db6" />
<img width="656" height="149" alt="image" src="https://github.com/user-attachments/assets/c817388f-656f-47f8-a4ec-17a4a028d343" />

##creamos la parte de mantenimiento y su index.html
<img width="736" height="22" alt="image" src="https://github.com/user-attachments/assets/3232b16a-728a-485a-b8f9-1c80c6b88389" />

<img width="879" height="279" alt="image" src="https://github.com/user-attachments/assets/6ae6b57a-b66c-4a81-a400-f0a8770f816d" />
## editamos el .conf de mantenimiento
<img width="712" height="474" alt="image" src="https://github.com/user-attachments/assets/319cf9ee-44b2-4088-8fe8-116306c105ac" />
## y tambien en el conf de la web1 para el redireccionamiento
<img width="736" height="480" alt="image" src="https://github.com/user-attachments/assets/97f3cd18-b2d7-446e-ae54-68cdc5c4f804" />
## ahora con esta configuracion cada vez que busquemos la pagina web1 no redirige automáticamente hacia el https y no podremos ver lo anterior
<img width="1202" height="245" alt="image" src="https://github.com/user-attachments/assets/d8fffd3f-3a61-4da1-b9b6-5def4b0637c5" />
