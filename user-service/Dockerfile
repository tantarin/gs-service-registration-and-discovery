# Используем официальный образ JDK
FROM eclipse-temurin:23-jdk
RUN apt-get update && apt-get install -y curl

# Указываем рабочую директорию
WORKDIR /app

# Копируем JAR файл из target в рабочую директорию контейнера
COPY target/user-service-0.0.1-SNAPSHOT.jar user-service.jar

# Указываем команду для запуска приложения
ENTRYPOINT ["java", "-jar", "/app/user-service.jar"]

# Открываем порт для доступа
EXPOSE 8081
