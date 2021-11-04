# Пример использования Liquibase

1. Установите базу данных MySQL на компьютер (либо используйте другую базу данных, но в таком случае необходимо изменить драйвер `spring.datasource.driver-class-name` в файле `src/main/resources/application.properties`)
2. В файле `src/main/resources/application.properties` укажите username и password для входа в MySQL
3. В корне проекта запустите эту команду. Данная команда запустит выполнение changeSet-ов из файла `src/main/resources/db/changelog/liquibase-changeLog.xml`:
```
mvnw liquibase:update
```
