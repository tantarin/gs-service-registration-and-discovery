# Используем официальный образ JDK
FROM eclipse-temurin:23-jdk

# Указываем рабочую директорию
WORKDIR /app

# Копируем JAR файл из target в рабочую директорию контейнера
COPY target/user-service.jar user-service.jar

# Указываем команду для запуска приложения
ENTRYPOINT ["java", "-jar", "/app/user-service.jar"]

# Открываем порт для доступа
EXPOSE 8081
