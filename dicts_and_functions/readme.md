## Практические задания для самостоятельного выполнения Словари и Функции. №8
- ### Начальный уровень
  - #### Задание №1
    1. Создайте пустой словарь с именем my_dict.
    2. Добавьте в словарь my_dict следующие элементы:
       | Ключ | Значение |
       |:----:|:--------:| 
       | "name" | "John" |
       | "age" | 25 |
       | "city" | "New York" |
    4. Выведите на экран содержимое словаря my_dict.
    5. Измените возраст в словаре my_dict на 26.
    6. Добавьте ключ "email" со значением "john@example.com" в словарь my_dict.
    7. Удалите ключ "city" из словаря my_dict.
    8. Выведите на экран все ключи и значения из словаря my_dict

- ### Базовый уровень
  - #### Задание №1
    1. Создайте пустой словарь с именем my_dict.
    2. Добавьте в словарь my_dict следующие элементы:
       | Ключ | Значение |
       |:----:|:--------:| 
       | "name" | "John" |
       | "age" | 25 |
       | "city" | "New York" |
    4. Выведите на экран содержимое словаря my_dict.
    5. Измените возраст в словаре my_dict на 26.
    6. Добавьте ключ "email" со значением "john@example.com" в словарь my_dict.
    7. Проверьте, есть ли ключ "country" в словаре my_dict, и выведите соответствующее сообщение.
    8. Выведите на экран все ключи и значения из словаря my_dict

## Примеры ввода/вывода 
- ### Начальный уровень
  - #### Задание №1
    | Ввод  | Вывод |
    |:------------------------:|:---------------:|
    | *отсутствует* | {"name": "John", "age": 25, "city": "New York"} <br> Ключ: name, Значение: John <br> Ключ: age, Значение: 26 <br> Ключ: email, Значение: john@example.com |
- ### Базовый уровень
  - #### Задание №1
    | Ввод  | Вывод |
    |:------------------------:|:---------------:|
    | *отсутствует* | {"name": "John", "age": 25, "city": "New York"} <br> Ключ 'country' отсутствует <br> Ключ: name, Значение: John <br> Ключ: age, Значение: 26 <br> Ключ: city, Значение: New York <br> Ключ: email, Значение: john@example.com |

## Алгоритмы решения
- ### Начальный уровень
  - #### Задание №1
    1. Создаем переменную my_dict, в которой храниться пустой словарь
    ```py
    # пустой словарь - {}
    my_dict = {}
    ```
    2. Добавить в словарь my_dict элементы
    ```py
    # элементы добавляются по шаблону
    # словарь["ключ"] = Значение
    my_dict["name"] = 'John'
    my_dict["age"] = 25
    my_dict["city"] = "New York"
    ```
    3. Вывести словарь
    ```py
    print(my_dict)
    ```
    4. Изменить значение в my_dict по ключу "age" на 26
    ```py
    my_dict["age"] = 26
    ```
    5. Добавим ключ "email" со значением "john@example.com" в словарь my_dict
    ```py
    my_dict["email"] = "john@example.com"
    ```
    6. Удаляем ключ "city" из словаря.
    ```py
    # pop() - функция в массивах, удаление элемента по индексу или ключу.
    my_dict.pop('city')
    7. Выводим на экран все ключи и значения в определенном формате с помощью цикла for
    ```py
    # my_dict.items() - это 2 перебираемых (списка с ключами и их значениями?)
    # key, value - переменные с ключами и значениями.
    for key, value in my_dict.items():
      print(f'Ключ: {key}, Значение: {value}')
    ```
- ### Базовый уровень
  - #### Задание №1
    1. Создаем переменную my_dict, в которой храниться пустой словарь
    ```py
    # пустой словарь - {}
    my_dict = {}
    ```
    2. Добавить в словарь my_dict элементы
    ```py
    # элементы добавляются по шаблону
    # словарь["ключ"] = Значение
    my_dict["name"] = 'John'
    my_dict["age"] = 25
    my_dict["city"] = "New York"
    ```
    3. Вывести словарь
    ```py
    print(my_dict)
    ```
    4. Изменить значение в my_dict по ключу "age" на 26
    ```py
    my_dict["age"] = 26
    ```
    5. Добавим ключ "email" со значением "john@example.com" в словарь my_dict
    ```py
    my_dict["email"] = "john@example.com"
    ```
    6. Проверяем есть ли ключ "country" и выводим Ключ "country" присутствует/отсутствует в словаре 
    ```py
    # Используем тернистый оператор
    # get() - функция в словаре, получает значение ключа (1-го аргумента), если ключ отсутствует, то возращает None (2-й аргумент)
    print("Ключ 'country' отсутствует" if my_dict.get("country", None) == None else "Ключ 'country' присутсвует")
    ```
    7. Выводим на экран все ключи и значения в определенном формате с помощью цикла for
    ```py
    # my_dict.items() - это 2 перебираемых (списка с ключами и их значениями?)
    # key, value - переменные с ключами и значениями.
    for key, value in my_dict.items():
      print(f'Ключ: {key}, Значение: {value}')
    ```
