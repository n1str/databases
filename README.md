# Учебный проект по базам данных

## Описание проекта

Данный репозиторий содержит набор учебных баз данных и SQL-запросов, разработанных в рамках домашнего задания по дисциплине "База данных". Проект включает в себя четыре различные базы данных, каждая из которых моделирует определенную предметную область и содержит набор SQL-запросов для решения различных задач.

## Структура репозитория

Репозиторий организован в виде четырех основных директорий, каждая из которых представляет отдельную базу данных:

### 1. database_booking_hotel
База данных для системы бронирования отелей.

**Структура базы данных:**
- `Hotel` - таблица с информацией об отелях
- `Room` - таблица с информацией о номерах в отелях
- `Customer` - таблица с информацией о клиентах
- `Booking` - таблица с информацией о бронированиях

**Файлы:**
- `db_create.sql` - скрипт создания таблиц
- `db_insert.sql` - скрипт наполнения таблиц данными
- `db_task1.sql`, `db_task2.sql`, `db_task3.sql` - SQL-запросы для решения задач

### 2. database_car_races
База данных для системы учета автомобильных гонок.

**Структура базы данных:**
- `Classes` - таблица с информацией о классах автомобилей
- `Cars` - таблица с информацией об автомобилях
- `Races` - таблица с информацией о гонках
- `Results` - таблица с результатами гонок

**Файлы:**
- `db_create.sql` - скрипт создания таблиц
- `db_insert.sql` - скрипт наполнения таблиц данными
- `db_task1.sql` - `db_task5.sql` - SQL-запросы для решения задач

### 3. database_company_structure
База данных для системы управления структурой компании.

**Структура базы данных:**
- `Departments` - таблица с информацией об отделах
- `Roles` - таблица с информацией о ролях
- `Employees` - таблица с информацией о сотрудниках
- `Projects` - таблица с информацией о проектах
- `Tasks` - таблица с информацией о задачах

**Файлы:**
- `db_create.sql` - скрипт создания таблиц
- `db_insert.sql` - скрипт наполнения таблиц данными
- `db_task1.sql`, `db_task2.sql`, `db_task3.sql` - SQL-запросы для решения задач

### 4. database_vehicle
База данных для системы учета транспортных средств.

**Структура базы данных:**
- `Vehicle` - таблица с общей информацией о транспортных средствах
- `Car` - таблица с информацией об автомобилях
- `Motorcycle` - таблица с информацией о мотоциклах
- `Bicycle` - таблица с информацией о велосипедах

**Файлы:**
- `db_create.sql` - скрипт создания таблиц
- `db_insert_data.sql` - скрипт наполнения таблиц данными
- `db_task1.sql`, `db_task2.sql` - SQL-запросы для решения задач

## Цели и задачи проекта

Основные цели проекта:
1. Практическое применение знаний по проектированию баз данных
2. Разработка SQL-запросов различной сложности

Задачи, решаемые в рамках проекта:
- Создание структуры таблиц с использованием первичных и внешних ключей
- Наполнение таблиц тестовыми данными
- Разработка сложных SQL-запросов с использованием JOIN, GROUP BY, подзапросов

## Инструкция по запуску

Для работы с базами данных и выполнения SQL-запросов вам потребуется:

1. СУБД MySQL или MariaDB (версия 5.7 или выше)
2. MySQL Workbench или другой клиент для работы с MySQL

### Порядок действий:

1. Клонируйте репозиторий:
   ```
   git clone https://github.com/n1str/databases.git
   ```

2. Для каждой базы данных выполните следующие шаги:
   - Откройте MySQL Workbench и подключитесь к вашему серверу MySQL
   - Создайте новую базу данных для каждого проекта:
     ```sql
     CREATE DATABASE database_booking_hotel;
     CREATE DATABASE database_car_races;
     CREATE DATABASE database_company_structure;
     CREATE DATABASE database_vehicle;
     ```
   - Выберите соответствующую базу данных:
     ```sql
     USE database_name;
     ```
   - Выполните скрипт создания таблиц (`db_create.sql`)
   - Выполните скрипт наполнения данными (`db_insert.sql` или `db_insert_data.sql`)
   - Выполните SQL-запросы из файлов `db_task*.sql` для проверки работоспособности

## Заключение

Данный проект демонстрирует навыки проектирования баз данных и написания SQL-запросов различной сложности. Каждая база данных представляет собой отдельную предметную область с уникальной структурой и набором задач, что позволяет продемонстрировать разнообразные подходы к работе с данными.
