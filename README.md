# **Propuesta de examen de Docker y Contenedores**

1\. ¿Cuál es la definición más precisa de un contenedor?  
A) Una máquina virtual ligera con hardware emulado.  
B) Una unidad de software estandarizada que empaqueta código y dependencias para que la aplicación se ejecute de forma rápida y confiable.  
C) Un archivo comprimido que solo funciona en sistemas operativos Linux con interfaz gráfica.  
D) Un servidor físico dedicado exclusivamente a una aplicación web.

---

2\. ¿Cuál es el principal objetivo de la plataforma Docker?  
A) Reemplazar por completo el uso de sistemas operativos en servidores.  
B) Proveer un lenguaje de programación único para aplicaciones en la nube.  
C) Construir, distribuir y ejecutar aplicaciones en contenedores de manera sencilla.  
D) Gestionar únicamente la seguridad de las redes de área local.  

---

3\. ¿Cuál es la diferencia fundamental entre una imagen y un contenedor?  
A) El contenedor es el molde estático y la imagen es el proceso en ejecución.  
B) No hay diferencia técnica; ambos términos son sinónimos en Docker.  
C) La imagen es un conjunto de ficheros empaquetados (molde) y el contenedor es la instancia de esa imagen en ejecución.  
D) Las imágenes solo existen en registros externos y los contenedores solo en el disco duro local.

---

4\. ¿Qué componentes del Kernel de Linux utiliza Docker para garantizar el aislamiento y límite de recursos?  
A) El sistema de archivos EXT4 y protocolos SSH.  
B) Namespaces y Cgroups (Control Groups).  
C) Direcciones IP estáticas y memoria SWAP.  
D) El Firewall de Linux y certificados SSL.

---

5\. ¿Qué herramienta se recomienda instalar en entornos sin interfaz gráfica?  
A) Docker Desktop.  
B) Docker Cloud.  
C) Docker Engine.  
D) Docker Dashboard.

---

6\. En cuanto a las suscripciones de Docker, ¿cuál es el coste para un estudiante o para proyectos personales?  
A) Una cuota mensual reducida.  
B) Es gratuito bajo la suscripción "Docker Personal".  
C) Requiere una suscripción "Business" obligatoria.  
D) Solo es gratuito durante un periodo de prueba de 30 días.

---

7\. ¿Qué comando se utiliza para listar únicamente los contenedores que están actualmente en ejecución?  
A) docker container list-all  
B) docker container ls  
C) docker ps \-all  
D) docker container show

---

8\. ¿Qué parámetro se debe añadir al comando de listado para ver todos los contenedores, incluidos los detenidos?  
A) \-v  
B) \--stopped  
C) \-a (o \--all)  
D) \--show-all 

---

9\. ¿Qué comando permite conocer el consumo de CPU y memoria de los contenedores en tiempo real?  
A) docker system df  
B) docker container stats  
C) docker image inspect  
D) docker container top

---

10\. Para consultar el espacio en disco utilizado por imágenes, contenedores y volúmenes, ¿qué comando se utiliza?  
A) docker system df  
B) docker container ls \-s  
C) docker image space  
D) docker volume inspect  

---

11\. ¿Cómo se estructuran las imágenes de Docker según el libro?  
A) Como un único bloque de datos comprimido e indivisible.  
B) Mediante capas (layers), donde cada capa representa cambios en la estructura de ficheros.  
C) En una jerarquía de carpetas similar a la de un sistema Windows.  
D) Como una base de datos relacional de archivos. 

---

12\. ¿Qué instrucción de un Dockerfile es obligatoria para definir la imagen base de la que partimos?  
A) BASE  
B) START  
C) FROM  
D) SOURCE  

---

13\. ¿Qué comando permite visualizar el historial de capas e instrucciones utilizadas para crear una imagen?  
A) docker image history  
B) docker image layers  
C) docker inspect \--build  
D) docker image logs  

---

14\. ¿Cuál es el nombre predeterminado que Docker busca al ejecutar un comando de construcción (build)?  
A) docker.yaml  
B) Dockerfile  
C) build.sh  
D) container.conf

---

15\. Si el archivo de construcción tiene un nombre distinto al estándar, ¿qué parámetro se usa en el comando build?  
A) \--name  
B) \-f (o \--file)  
C) \-t  
D) \--context 

---

16\. ¿Qué parámetro permite especificar la arquitectura de hardware (ej. linux/arm64) durante la construcción?  
A) \--arch  
B) \--system  
C) \--platform  
D) \--target  

---

17\. ¿Cuál es la principal ventaja de utilizar la técnica "multi-stage build" en un Dockerfile?  
A) Permite ejecutar varios contenedores al mismo tiempo.  
B) Ayuda a obtener imágenes finales mucho más pequeñas y limpias al separar el entorno de compilación.  
C) Aumenta la velocidad de descarga de las imágenes desde Docker Hub.  
D) Permite que la imagen funcione sin necesidad de tener instalado Docker Engine.  

---

18\. ¿Qué versión de Docker Compose se analiza principalmente en el libro y se usa como plugin del CLI?  
A) Docker Compose V1.  
B) Docker Compose V2.  
C) Docker Compose Pro.  
D) Docker Swarm.  

---

19\. ¿Qué comando de Compose permite construir la imagen (si es necesario) y arrancar los servicios en un solo paso?  
A) docker compose start  
B) docker compose run  
C) docker compose up  
D) docker compose build  

---

20\. Si necesitas forzar la construcción de las imágenes cada vez que levantas los servicios, ¿qué parámetro usas?  
A) \--rebuild  
B) \--build  
C) \--force  
D) \--new  

---

21\. ¿Cómo se ejecutan los servicios de Compose en segundo plano (background) para liberar la terminal?  
A) Con el parámetro \--background  
B) Con el parámetro \--silent  
C) Con el parámetro \-d (o \--detach)  
D) Con el parámetro \-b  

---

22\. Según las buenas prácticas de la V2, ¿cuál es el nombre preferido para el archivo de configuración de Compose?  
A) docker-compose.yml  
B) compose.yaml  
C) services.json  
D) docker-stack.xml  

---

23\. En un archivo de Compose, ¿qué representa la instrucción context dentro de la sección build?  
A) La versión del motor de Docker necesaria.  
B) La carpeta o ruta que se toma como referencia para buscar el Dockerfile y los archivos.  
C) El nombre del autor del contenedor.  
D) El puerto de red que se va a abrir al exterior. 

---

24\. ¿Qué directiva se usa para establecer que un servicio dependa de que otro se inicie primero (ej. una DB)?  
A) links  
B) networks  
C) depends\_on  
D) priority  

---

25\. ¿Qué comando permite obtener toda la información técnica detallada de una imagen en formato JSON?  
A) docker image ls  
B) docker image inspect  
C) docker image check  
D) docker image detail  

---

26\. ¿Qué sucede con los datos escritos dentro de un contenedor si este es eliminado y no se usaron volúmenes?  
A) Se guardan automáticamente en Docker Hub.  
B) Permanecen ocultos en el sistema operativo host.  
C) Se pierden definitivamente.  
D) Se recuperan automáticamente al crear un nuevo contenedor con el mismo nombre.  

---

27\. ¿Cuál de estos es un registro donde se pueden publicar y compartir imágenes de Docker?  
A) Docker Hub.  
B) ttl.sh (para imágenes efímeras).  
C) Registros privados (Azure, AWS, Google).  
D) Todas las anteriores son correctas.  

---

28\. ¿Qué comando se utiliza para detener un contenedor que está en ejecución sin borrarlo?  
A) docker container stop  
B) docker container rm  
C) docker container pause  
D) docker container end  

---

29\. Para eliminar de una sola vez contenedores detenidos, redes no usadas e imágenes sin nombre (dangling), usamos:  
A) docker system clean  
B) docker system prune  
C) docker system delete  
D) docker system clear  

---

30\. ¿Cuál es la ventaja principal de usar redes (networks) personalizadas en Docker?  
A) Permite que los contenedores se comuniquen entre sí usando sus nombres como DNS internos.  
B) Aumenta la velocidad de conexión a internet de la máquina host.  
C) Evita que tengamos que instalar drivers de red en el ordenador.  
D) Es la única forma de que un contenedor pueda acceder a una base de datos externa.

---

### 

### **Respuestas:**

1-B, 2-C, 3-C, 4-B, 5-C, 6-B, 7-B, 8-C, 9-B, 10-A, 11-B, 12-C, 13-A, 14-B, 15-B, 16-C, 17-B, 18-B, 19-C, 20-B, 21-C, 22-B, 23-B, 24-C, 25-B, 26-C, 27-D, 28-A, 29-B, 30-A.
