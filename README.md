# Salesman
SalesmanUI - интерфейс для задания точек и отображения решения (ui)  
SalesmanCount - поиск минимального пути путем рандома (прожка обсчета)  
Как пользоваться:  
0. Задать пути к файлам, через которые ui и прожка обсчета будут обмениваться информацией:  
-exportPath и importPath в файле App.config SalesmanUI. По пути exportPath будут сохраняться заданные для обсчета точки, по importPath загружаться результат  
-inputPath и outputPath прямо в функции main SalesmanCount  - соответственно inputPath=exportPath из предыдущего пункта, outputPath=importPath  
(Да, такой вот хардкод, дешево, сердито, для зачета)  
1. Запустить SalesmanUI (например в студии)  
2. Левой кнопкой натыкать точек на панели SourceData
3. Кликнуть export 
4. Запустить exeшник SalesmanCount командой mpiexec -n N SalesmanCount.exe, где N - количество процессов.
5. Дождаться вывода результатов в консоль
6. Кликнуть import в SalesmanUI

Готово, вы великолепны
Можно использовать только SalesmanCount, а интерфейс сделать самим, эти прожки независимы в общем.
