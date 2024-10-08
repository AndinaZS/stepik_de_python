# Задание #
### Реализовать следующие функции: ###

1. **read_sales_data(file_path)**, которая принимает путь к файлу и возвращает список продаж.  
Продажи в свою очередь являются словарями с ключами product_name, quantity, price, date (название, количество, цена, дата).
2. **total_sales_per_product(sales_data)**, которая принимает список продаж и возвращает словарь,  
где ключ - название продукта, а значение - общая сумма продаж этого продукта.
3. **sales_over_time(sales_data)**, которая принимает список продаж и возвращает словарь,  
где ключ - дата, а значение общая сумма продаж за эту дату.  

Входные данных должны храниться в файле (файл должен быть в том же репозитории проекта.  

<ins>В ходе анализа данных из файла необходимо вывести на экран два значения:</ins>

1. Определить, какой продукт принес наибольшую выручку.
2. Определить, в какой день была наибольшая сумма продаж.
 

<ins>В завершении работы вашей программы необходимо построить два графика:</ins>

1. Построить график общей суммы продаж по каждому продукту.
2. Построить график общей суммы продаж по дням.

## Информация по результату ##

### Требования к запуску приложения: ###
- версия Python не ниже 3.10
- установить зависимости из файла requirements.txt
- файлы для анализа должны находиться в рабочей директории, иметь формат txt или csv, разделение - запятые.

### Работа приложения: ###
В файле main.py происходит вызов функции get_result, на вход которой необходимо подать путь к файлу (get_result('test.csv'))  
В результате работы будет выведено окно с графиками и запрошенной информацией из задания  
(окно лучше развернуть на весь экран, с масштабированием не срослось).  

При работе get_result происходит вызов функций, указанных в задании. При необходимости, их можно вызвать отдельно (закомменчено).  

### Примечания: ###
1. сделана примитивная проверка на существование файла
2. сделана построчная проверка на корректность данных (количество значений в строке и тип для чисел).  
При некорректно считанной строке выводится информация с номером строки.
