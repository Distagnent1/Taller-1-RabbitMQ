# Taller RabbitMQ
En esta actividad haremos uso de Java y Node para los productores y consumidores. La carpeta principal del proyecto se divide de la siguiente manera:

![Imagen](https://i.postimg.cc/rwPMJJH1/2024-09-17-08-49.png)

El Docker Compose lo configuramos para que reinicie todos los contenedores en caso de que suceda algún imprevisto o se apaguen, así aseguramos que siempre estén funcionando.

![Imagen](https://i.postimg.cc/MHPFSsVt/2-Configurar-Reinicio-de-los-Contenedores.png)

En el caso de los productores, definimos un intervalo de cinco segundos para el envío de mensajes automático.

![Imagen](https://i.ibb.co/c3gtXhH/3-1-Definir-Intervalo-de-Cinco-Segundos-para-el-Publisher-Java.png)

![Imagen](https://i.ibb.co/GHt6vLL/3-2-Programar-el-Env-o-del-Mensaje-cada-Cinco-Segundos.png)

![Imagen](https://i.ibb.co/xHFsX4Y/4-Programar-el-Env-o-del-Mensaje-cada-Cinco-Segundos-Node.png)

Con la aplicación Docker Desktop verificamos que todos los contenedores estén funcionando.

![Imagen](https://i.ibb.co/f8w8jb2/5-Contenedores-Funcionando.png)

En la terminal de Visual Studio Code vemos cómo los publicadores están enviando los mensajes cada cinco segundos y los consumidores les responden.

![Imagen](https://i.ibb.co/yShfQfz/6-Env-o-y-Recepci-n-de-Mensajes.png)

Finalmente, si ingresamos a RabbitMQ con las credenciales de guest para usuario y contraseña, en el "Overview" nos muestra una gráfica referente a los mensajes enviados y recibidos.

![Imagen](https://i.ibb.co/yNb0q7S/7-Gr-fica-de-Mensajes-en-Rabbit-MQ.png)
