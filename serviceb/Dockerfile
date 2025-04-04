# Используем официальный образ JDK
FROM eclipse-temurin:23-jdk

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем JAR файл из target в рабочую директорию контейнера
COPY target/order-service.jar order-service.jar

# Указываем команду для запуска приложения
ENTRYPOINT ["java", "-jar", "/app/order-service.jar"]

# Открываем порт для доступа
EXPOSE 8082
