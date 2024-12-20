# Reconocimiento y clasificación de tanques en el videojuego War Thunder
## Modelo basado en YOLOv8s entrenado con un set de datos personalizado para el reconocimiento y clasificación de tanques en War Thunder.
### El modelo fue entrenado con 471 imagenes de capturas de pantalla obtenidas dentro del juego, preprocesadas y aumentadas con mosaicos, rotaciones e inclinación, resultando en 1229 imagenes

### Para montar el compose, ejecutar el comando: docker-compose up -d
### Para iniciar la conexión local con Colab, ejecutar el comando docker logs yolo_runtime y compiar el enlace con el token generado como:  http://127.0.0.1:9000/?token=XXXXXXXXXXXXXXX
### Posteriormente insertar el token en el apartado para conectar a un entorno de ejecución local estando dentro de un google colab Notebook con el archivo .ipynb

### Insertar dentro de la carpeta models el archivo best.pt para cargar el modelo preentrenado
### En caso de querer seguir entrenando el modelo, insertar dentro de la carpeta data el archivo data.yaml junto con con los directorios "train", "valid" y "test" 
### En caso de querer realizar una predicción, insertar en la carpeta images las imagenes y reemplazar en el bloque N°6 la ruta hacia la imagen