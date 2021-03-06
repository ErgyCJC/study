# Задача 4. Супер-массив строк

## Условие

Реализуйте структуру данных “массив строк” на основе декартового дерева по неявному ключу со следующими методами:

+ Добавление строки в позицию position. Все последующие строки сдвигаются на одну позицию вперед.\
`void InsertAt( int position, const std::string& value );`

+ Удаление строки из позиции position. Все последующие строки сдвигаются на одну позицию назад.\
`void DeleteAt( int position );`

+ Получение строки из позиции position.\
`std::string GetAt( int position );`

Все методы должны работать за O(log n) в среднем, где n – текущее количество строк в массиве.

## Формат ввода

Первая строка содержит количество команд k <= 10^6.

Последующие k строк содержат описания команд:

+ Команда `+ 10 hello` означает добавление строки hello в позицию 10.

+ Команда `- 14 16` означает удаление строки от позиции 14 до позиции 16.

+ Команда `- 13` означает удаление строки в позии 13

+ Команда `? 33` означает запрос на вывод строки из массива в позиции 33.

## Формат вывода

Выведите все строки, запрошенные командами `?`.

## Пример


##### Ввод:
```
6
+ 0 myau
+ 0 krya
? 0
+ 2 gav
- 1 1
? 1
```

##### Вывод:
```
krya
gav
```
