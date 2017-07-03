Following “The Principle of Least Surprise,”2 any function or class should implement the behaviors that another programmer could reasonably expect. For example, consider a function that translates the name of a day to an enum that represents the day.
2. Or “The Principle of Least Astonishment”: http://en.wikipedia.org/wiki/
         Principle_of_least_astonishment
```
   Day day = DayDate.StringToDay(String dayName);
```
We would expect the string “Monday” to be translated to Day.MONDAY. We would also expect the common abbreviations to be translated, and we would expect the function to ignore case.
When an obvious behavior is not implemented, readers and users of the code can no longer depend on their intuition about function names. They lose their trust in the original author and must fall back on reading the details of the code.”

[Espanol]
Siguiendo el principio de al menos una sorpresa, cualquier funcion o clase deberia implementar comportamiento que otros programadores pudieran rasonablemente esperar. Por ejemplo, considera una funcion que traduce el nombre de un dia a un numero que representa el dia:
```
Dia dia = DiaFecha.StringADia(String NombreDia);
``` 
nos gustaria recibir la cadena ```"Lunes"``` para ser traducida a ```Dia.LUNES``` nos gustaria recibir una abreviacion comun para se traducida, y ademas que la funcion  ignore el caso.
cuando un comportamiento obvio no es implementado, los lectores y usuarios del codigo pueden ya no depender de su intuicion acerca del nombre de las funciones. Ellos pierden la confianza en  el autor original y se ven obligados a volver a leer los detalles del codigo

Excerpt From: Martin, Robert C. “Clean Code: A Handbook of Agile Software Craftsmanship.” iBooks. 