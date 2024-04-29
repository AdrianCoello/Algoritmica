# Programa: Uso de la Clase list en C++
Este programa ilustra cómo utilizar la clase **list** en C++. La clase **list** proporciona una implementación de una lista doblemente enlazada. 
A continuación, se explica el funcionamiento del código:

# Creación de una Lista (listita):
Se crea una instancia de la clase list llamada listita.
Se agregan tres elementos (1, 2 y 3) al final de la lista utilizando push_back().
Iteración a través de la Lista:
Se declara un iterador de tipo list<int>::iterator llamado it.
Se inicializa it con el valor de listita.end(), que apunta al elemento después del último elemento de la lista.
Se imprime el valor apuntado por it. En este caso, será un valor no definido (basura).
Luego, se itera a través de la lista utilizando un bucle for. El iterador it se mueve desde el principio (listita.begin()) hasta el final (listita.end()).
En cada iteración, se imprime el valor apuntado por it.
