# JVM
![](https://github.com/sualval/JVM/blob/main/document.jpg)

* В ClassLoader передаются системные и созданые класы проверяются и загружаются в Metaspace
* В момент вызова метода main ,в Stack создается фрейм.
* Туда  сохраняются int i=1 переменная,ссылка на Object o, Integer ii -Объекты добавляются в Heap.
* В момент вызова метода printAll ,в Stack создается фрейм.
* Туда копируются ссылки и переменные из main и создается новая ссылка uselessVar на integer.
* В момент вызова метода println ,в Stack создается фрейм.
* Туда копируются int i=1 переменная, ссылка на  Integer. 
* Создается ссылка на String преобразованная из Object.\
(метод toString создает фрейм с Object отдает String в  println и уничтожается )
* В Heap добавляется объект String.
* Далее из Stack удаляются все фреймы.
* Создается новый фрейм println с ссылкой на String,который добавляется в Heap.
* Stack пустой. 
