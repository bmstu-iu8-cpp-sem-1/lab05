## Лабораторная работа 5

### Инструкция
Каждое задание должно быть выполненно в отдельном `.cpp` файле.
Прототипы функции должны быть вынесены в соответствующие `.hpp` файлы.
Все реализованные функции необходимо вызвать в фунции `main` в файле [lab05](lab05.cpp)
Все `.cpp` файлы добавить в `CMakeLists.txt`

### Задание
1. Необходимо реализовать функцию, которая определяет арифметическое средее в массиве.
Прототип функции:
```cpp
float mean(const std::vector<float>&);
```

1. Необходимо реализовать функцию, которая определяет максимум и минимум в массиве. 
Прототип функции:
```cpp
// .first is min
// .second is max
std::pair<float, float> minMax(const std::vector<float>&);
```

1. Необходимо реализовать функцию `argmax`, которая определяет индекс максимума в массиве. 
Прототип функции необходимо выбрать самостоятельно.

1. Необходимо реализовать функцию, которая сортирует входной массив.
Прототип функции:
```cpp
void sort(std::vector<float>&);
```

1. Необходимо реализовать функцию, которая удаляет первый отрицательный элемент. Удаленный элемент необходимо вернуть.
Прототип функции необходимо выбрать самостоятельно.

1. Необходимо реализовать функцию, заменяет в строке все вхождения подстроки на новую строку.
```cpp
std::string replace(const std::string& str, const std::string& old, const std::string& new);
```
Пример:
```cpp
std::string newString = replace("Can you can a can as a canner can can a can?", "can", "cAN");
std::cout << newString; // "Can you cAN a cAN as a cANner cAN cAN a cAN?"
```

1. Необходимо реализовать функцию, которая делит строку по задонному символу.
```cpp
std::vector<std::string> split(const std::string&, char sep = ' ');
```
Пример:
```cpp
std::vector<std::string> arr = split("Can you can a can as a canner can can a can?", ' ');
// arr == {"Can", "you", "can", "a", "can", "as", "a", "canner", "can", "can", "a", "can?"};
```

1. Необходимо реализовать функцию, которая соединяет массив строк в одну строку.
```cpp
std::string join(const std::vector<std::string>&, const std::string& sep);
```
Пример:
```cpp
std::vector<std::string> arr = {"Can", "you", "can", "a", "can", "as", "a", "canner", "can", "can", "a", "can?"};
std::string str = join(arr, " ");
// str == "Can you can a can as a canner can can a can?"
```
