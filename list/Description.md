## Домашнее задание Списки. №5
- ### Начальный уровень
  - #### Задание №1
    1. Создайте список из 10 элементов с разными типами данных (строки, числа и булевы значения) и выведите его на экран.
    2. Используя срезы, выведите на экран первые 5 элементов списка, последние 3 элемента списка и каждый второй элемент списка. (разделение между срезами новой строкой)
    3. Измените 3 элемент списка на новое значение и выведите измененный список на экран.

- ### Базовый уровень
  - #### Задание №1
      1. Создайте список из 10 элементов с разными типами данных (строки, числа и булевы значения) и выведите его на экран.
      2. Используя срезы, выведите на экран первые 5 элементов списка, последние 3 элемента списка и каждый второй элемент списка.
      3. Измените 3 элемент списка на новое значение и выведите измененный список на экран.
  - #### Задание №2
      1. Попросите пользователя ввести число с клавиатуры.
      2. Выведите сообщение, зависящее от условия:
          - Если число делится на 3 без остатка, то "Число делится на 3".
          - Если число больше 10, то "Число больше 10".
          - Если число не удовлетворяет ни одному из условий, выведите сообщение "Число не соответствует условиям".

## Примеры ввода/вывода 
- ### Начальный уровень
  - #### Задание №1
    | Ввод  | Вывод |
    |:------------------------:|---------------|
    | *отсутствует* | [1, 1.11, 'Bye, World!', '1', {1.1, 11}, (111, 0.1), [1, 0], {'city': 'Москва', 'name': 'Павел'}, True, False, 'Python'] <br> [1, 1.11, 'Bye, World!', '1',  {1.1, 11}] <br> [True, False, 'Python'] <br> [1.11, '1', (111, 0.1), {'city': 'Москва', 'name': 'Павел'}, False] <br> [1, 1.11, 'Hello, World!', '1', {1.1, 11}, (111, 0.1), [1, 0], {'city': 'Москва', 'name': 'Павел'}, True, False, 'Python']  |

- ### Базовый уровень
  - #### Задание №1
    | Ввод  | Вывод |
    |:------------------------:|---------------|
    | *отсутствует* | [1, 1.11, 'Bye, World!', '1', {1.1, 11}, (111, 0.1), [1, 0], {'city': 'Москва', 'name': 'Павел'}, True, False, 'Python'] <br> [1, 1.11, 'Bye, World!', '1',  {1.1, 11}] <br> [True, False, 'Python'] <br> [1.11, '1', (111, 0.1), {'city': 'Москва', 'name': 'Павел'}, False] <br> [1, 1.11, 'Hello, World!', '1', {1.1, 11}, (111, 0.1), [1, 0], {'city': 'Москва', 'name': 'Павел'}, True, False, 'Python']  |
  - #### Задание №2
    | Ввод  | Вывод |
    |:------------------------:|---------------|
    | *Введите число*: 3 | Число делится на 3 |
    | *Введите число*: 12 | Число делится на 3 <br> Число больше 10 |
    | *Введите число*: 13 | Число больше 10 |
    | *Введите число*: 2 | Число не соответствует условиям |

## Алгоритмы решения
- ### Начальный уровень
  - #### Задание №1
    1. Создадим переменную data, которая хранит список с 10 разными элементами, разных типов
    ```py
    # Хранит типы [int, float, str, str, set, tuple, list, dict, bool, bool, str]
    data = [1,  1.11, "Bye, World!", "1", {11, 1.1}, (111, 0.1), [1, 0], {"city": "Москва", "name": "Павел"}, True, False, "Python"]
    ```
    2. Выводим срезы с разделителем на строки
    ```py
    # Выводим сначала полный список, потом первые 5 элементов, дальше последние 3 элементов и в конце каждый 2 элемент
    # Используя параметр sep (separator) задаем ему разделитель \n
    print(data, data[:5], data[-3:], data[1::2], sep="\n")
    ```
    3. Изменяем 3 элемент в списке по индексу
    ```py
    # Изменяем 3 элемент "Bye, World!" на "Hello, World!"
    data[2] = "Hello, World!"
    ```
    4. Выводим измененный список
    ```py
    print(data)
    ```
- ### Базовый уровень
  - #### Задание №1
    1. Создадим переменную data, которая хранит список с 10 разными элементами, разных типов
    ```py
    # Хранит типы [int, float, str, str, set, tuple, list, dict, bool, bool, str]
    data = [1,  1.11, "Bye, World!", "1", {11, 1.1}, (111, 0.1), [1, 0], {"city": "Москва", "name": "Павел"}, True, False, "Python"]
    ```
    2. Выводим срезы с разделителем на строки
    ```py
    # Выводим сначала полный список, потом первые 5 элементов, дальше последние 3 элементов и в конце каждый 2 элемент
    # Используя параметр sep (separator) задаем ему разделитель \n
    print(data, data[:5], data[-3:], data[1::2], sep="\n")
    ```
    3. Изменяем 3 элемент в списке по индексу
    ```py
    # Изменяем 3 элемент "Bye, World!" на "Hello, World!"
    data[2] = "Hello, World!"
    ```
    4. Выводим измененный список
    ```py
    print(data)
    ```
  - #### Задание №2
    1. Создадим переменную number, которая хранит введенное число и is_cond, которая хранит булевое значение
    ```py
    # С помощью функции input() получаем ввод пользователя
    # С помощью функции int() меняем тип строка на целое число
    number = int(input())
    # создаем переменную is_cond, которая определяет выполнено одно из условий или нет
    # По умолчанию не выполнено (False)
    is_cond = False
    ```
    2. Создадим переменную conditions, хранящую список логических выражений.
    ```py
    # Список состоит из булевых значений True и False.
    conditions = [number % 3 == 0, number > 10]
    ```
    3. Используем цикл for для проверки условий и вывод сообщений
    ```py
    # цикл for, итерируемый объект range(len(conditions)), итератор i (число)
    # len() - функция возращающая количество элементов в списке
    # range(start, number, step) - функция возращающая итерируемый объект, список от start до number - 1 с шагом step, где start, number, step - числа, по умолчанию start=0, step=1.
    for i in range(len(conditions)):
      # если логическое выражение в списке по индексу i ложно, то
      if not conditions[i]:
        # начать следующую итерацию
        continue
      # если логическое выражение в списке по индексу i правдиво, то
      # Вывести значение в списке по индексу 0 или 1 (False или True)
      print(["Число делится на 3", "Число больше 10"][i == 1])
      # Так как логическое выражение правдиво, то is_cond равен True
      is_cond = True
    ```
    4. Выводим "Число не соответствует условиям", если число не удовлетворяет ни одному из условий
    ```py
    # Тернарный оператор.
    # Если значение is_cond НЕ правдиво, то выводим "Число не соответствует условиям"
    # Если нет, то ничего не выводим
    print("Число не соответствует условиям") if not is_cond else ''
    ```