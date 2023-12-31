## Практические задания для самостоятельного выполнения Структуры данных. №7
- ### Начальный уровень
  - #### Задание №1
    1. Создайте кортеж, содержащий три целых числа.
    2. Выведите на экран каждое число, а затем выведите их сумму.

- ### Базовый уровень
  - #### Задание №1
    1. Вводятся два списка чисел, числа вводятся пользователем.
    2. Выведите, сколько чисел содержится одновременно как в первом списке, так и во втором.

## Примеры ввода/вывода 
- ### Начальный уровень
  - #### Задание №1
    | Ввод  | Вывод |
    |:------------------------:|:---------------:|
    | *отсутствует* | Кортеж: (2, 4, 6) <br> Первое число: 2 <br> Второе число: 4 <br> Третье число: 6 <br> Сумма: 12|
- ### Базовый уровень
  - #### Задание №1
    | Ввод  | Вывод |
    |:------------------------:|:---------------:|
    | *Введите первый список:* 1 2 6 7 <br> *Введите второй список:* 2 7 5 9  | Количество пересечений: 2 |

## Алгоритмы решения
- ### Начальный уровень
  - #### Задание №1
    1. Определяем переменную data, которая содержит кортеж.
    ```py
    # кортеж содержит 3 элемента, типа int
    data = (2, 4, 6)
    ```
    2. С помощью индексов выводим числа кортежа
    ```py
    print(f'Первое число: {data[0]}\nВторое число: {data[1]}\nТретье число: {data[2]}')
    ```
    3. С помощью функции sum() выводим сумму элементов кортежа.
    ```py
    print(f'Сумма: {sum(data)}')
    ```
- ### Базовый уровень
  - #### Задание №1
    1. Определяем переменные data1, data2, которые содержат числа введенные пользователем.
    ```py
    # используем генератор множеств
    # split() - функция разделение строки на списки, используя по умолчанию делитель пробел
    # int() - функция преобразование из строки в целое число
    data1 = {int(i) for i in input("Введите первый список: ").split()}
    data2 = {int(i) for i in input("Введите второй список: ").split()}
    ```
    2. Выводим количество пересечений
    ```py
    # intersection() - функция множеств, нахождение пересечения множеств
    # len() - функция, возращающая количество элементов в массиве
    print(f'Количество пересечений: {len(data1.intersection(data2))}')
    ```
