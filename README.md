* 1
Ключевой класс проекта - SearchServer, имеющий конструктор, принимающий на вход поток ввода, содержащий базу документов (1 документ - 1 строка) и 2 метода: $\newline$ UpdateDocumentBase(istream& document_input) (меняет содержимое актуальной базы документов на содержимое document_input), $\newline$ AddQueriesStream(istream& query_input, ostream& search_results_output), выполняющий поиск по следующему принципу: запрос - строка query_input, результат поиска - строка в базе документов, имеющая наибольшее совпадение слов с query_input, выводится в document_input $\n$
Код предусматривает одновременную обработку запросов и обновления базы данных. То есть пока база данных обновляется, клиент сможет продолжать обрабатывать запросы 
* 2
Простая база данных, хранящая дату события (в формате year-month-day)  и событие (строку); функционал: добавить запись (add), удалить запись (del), найти запись по дате (find), вывести содержимое базы данных (print)
