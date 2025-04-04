# Используем официальный образ JDK
FROM eclipse-temurin:23-jdk

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем JAR файл из target в рабочую директорию контейнера
COPY target/eureka-server.jar eureka-server.jar

# Указываем команду для запуска приложения
ENTRYPOINT ["java", "-jar", "/app/eureka-server.jar"]

# Открываем порт для Eureka
EXPOSE 8761
