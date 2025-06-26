# Usa una imagen base oficial y moderna para Java 17
FROM eclipse-temurin:17-jdk-jammy

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Documenta el puerto en el que la aplicación escucha (generalmente 8080 para Spring Boot)
EXPOSE 8080

# Copia el archivo JAR desde la carpeta 'target' del contexto de construcción.
# Usar un comodín (*) hace que el Dockerfile sea independiente de la versión del proyecto.
COPY target/*.jar product-app.jar

# Define el comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "product-app.jar"]