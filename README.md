#HomeWork

<a href="https://ibb.co/C90tSJ7"><img src="https://i.ibb.co/wQ6L2JW/1st-task.png" alt="1st-task" border="0"></a>

0. Класс JvmComprehension, а также системные классы, загружаются с помощью ClassLoader в MetaSpace.  
0.1 В Stack Memory создается Frame public static void main(String[] args). 
Frame psvm()
1. В Frame psvm инициализируется локальная переменная int i = 1;
2. В Heap создается Object, в frame присваивается ссылка o на Object.
3. В Heap создается Integer, в frame присваивается ссылка ii на Integer.
Frame printAll()
4. В Stack Memory создается Frame printAll() с параметрами o (ссылка на Object), int i, ii (ссылка на Integer).
5. В Heap создается Integer, в frame присваивается ссылка uselessVar на Integer.
Frame system.out.println()
6. В Stack Memory создается Frame system.out.println() с параметрами o (ссылка на Object), int i, ii (ссылка на Integer).
6.1 Создается frame toString() с возврращаемым объектом типа String;
После обработки данных Stack Memory удаляет Frames в следующем порядке:
> toString, system.out.println, printAll
7. Создается frame system.out.println() с параметром String = finished;
После обработки данных Stack Memory удаляет Frames в следующем порядке:
> system.out.println, psvm.

Java программа завершает свою работу.


