# SIPI
# Документация разработчика AParts

## 1. Описание проекта
AParts — это веб-приложение для работы с каталогом автозапчастей. Система реализует функционал интернет-магазина: регистрацию пользователей, авторизацию, просмотр товаров, добавление в корзину и оформление заказов.


## 2. Архитектура приложения
Приложение построено по клиент-серверной архитектуре:

- Backend: Java + Spring Boot
- Frontend: Freemarker (шаблоны HTML)
- База данных: PostgreSQL

Используется REST-подход для взаимодействия компонентов.


## 3. Структура проекта
src/main/java/.../controller – REST-контроллеры
src/main/java/.../service – бизнес-логика
src/main/java/.../repository – доступ к базе данных
src/main/java/.../model – сущности (Entity)
src/main/resources/templates – HTML-шаблоны (Freemarker)


---

## 4. API документация

Для документирования API используется Swagger.

Swagger автоматически генерирует документацию на основе аннотаций в коде.

Доступ к документации: http://localhost:7483/swagger-ui.html


Документация включает:
- список эндпоинтов
- параметры запросов
- ответы сервера
- описание моделей данных

---

## 5. Запуск проекта

### Требования:
- Java 17+
- PostgreSQL
- Maven

### Шаги запуска:

1. Клонировать репозиторий:
   
2. Создать базу данных PostgreSQL

3. Настроить файл `application.properties`:
spring.datasource.url=jdbc:postgresql://localhost:5432/aparts
spring.datasource.username=postgres
spring.datasource.password=your_password

4. Запустить проект:
   mvn spring-boot:run
   
---

## 6. Используемые технологии

- Java 17
- Spring Boot
- Spring Security
- Spring Data JPA
- PostgreSQL
- Maven
- Freemarker
- Docker
- Swagger

---

## 7. Документирование

Документация разработчика формируется автоматически с помощью Swagger.

Преимущества:
- актуальность документации
- удобный интерфейс
- автоматическое обновление при изменении кода

---

## 8. Тестирование

Для тестирования используются:
- JUnit
- Mockito
- Postman / Swagger UI
