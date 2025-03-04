ru text
# Условия домашки
> Привет! На связи домашнее задание урока 4.5 параллельные стримы.

Цель сегодняшней домашней работы — написать несколько модификаторов для структур данных, используя Stream API.

### Шаг 1

Добавить эндпоинт для получения всех имен всех студентов, чье имя начинается с буквы А. В ответе должен находиться отсортированный в алфавитном порядке список с именами в верхнем регистре. Для получения всех студентов из базы использовать метод репозитория - 
findAll().

### Шаг 2

Создать эндпоинт, который будет возвращать средний возраст всех студентов. Для получения информации о всех студентах опять же следует использовать метод репозитория - 
findAll().

### Шаг 3

Создать эндпоинт, который будет возвращать самое длинное название факультета.

### Шаг 4

Создать эндпоинт (не важно в каком контроллере), который будет возвращать целочисленное значение. Это значение вычисляется следующей формулой:
```
int sum = Stream.iterate(1, a -> a +1) .limit(1_000_000) .reduce(0, (a, b) -> a + b );
```
Необходимо придумать способ уменьшить время ответа эндпоинта путем модификации вышеописанного выражения.

eng text
# Homework conditions
> Hello! The homework of lesson 4.5 is in touch with parallel streams.

The purpose of today's homework is to write several modifiers for data structures using the Stream API.

### Step 1

Add an endpoint to get all the names of all students whose name starts with the letter A. The response should contain an alphabetically sorted list with names in uppercase. To get all the students from the database, use the repository method. - 
findAll().

### Step 2

Create an endpoint that returns the average age of all students. To get information about all students, again, you should use the repository method. - 
findAll().

### Step 3

Create an endpoint that will return the longest faculty name.

### Step 4

Create an endpoint (no matter in which controller) that will return an integer value. This value is calculated using the following formula:
```
int sum = Stream.iterate(1, a -> a +1) .limit(1_000_000) .reduce(0, (a, b) -> a + b);
```
It is necessary to come up with a way to reduce the endpoint response time by modifying the expression described above.
