#Codigo DFS
El código implementa la búsqueda en profundidad (DFS) para determinar si un nodo (persona) puede llegar a otro en una red social (grafo). 
Imagina que cada persona es un nodo y las conexiones entre ellas son aristas. La DFS explora la red a partir de una persona (nodo inicial), siguiendo 
sus conexiones (vecinos) hasta llegar al objetivo (nodo final). Si la DFS marca al nodo final como visitado, significa que la persona inicial sí puede 
conocer a la persona final. El código utiliza una pila para ir explorando los nodos uno a uno, como si fuera una pila de platos que se va vaciando.
## Explicacion de codigo
### 1. Funcion dfs
Toma un nodoInicial como parámetro (la persona desde la que se inicia la búsqueda).
Utiliza una pila para almacenar los nodos a explorar (como una pila de platos).
Mientras la pila no esté vacía:
Obtiene el nodoActual de la pila (el primer plato por lavar).
Si el nodoActual no ha sido visitado:
Lo marca como visitado (ya lo lavamos).
Recorre sus vecinos (las personas a las que está conectado):
Si un vecino no ha sido visitado, lo agrega a la pila (lo ponemos en la pila para lavarlo después).
### 2. Función main:
Lee el número de nodos y aristas de la red social (cuántas personas y conexiones hay).
Lee las aristas y las almacena en la estructura grafo (conecta a las personas entre sí).
Lee los nodos inicial (S) y final (T) (la persona desde la que se inicia y la que se busca).
Llama a la función dfs con el nodo inicial S.
Si el nodo final T está marcado como visitado, imprime "Si lo podria conocer" (¡las dos personas están conectadas!).
De lo contrario, imprime "No lo podria conocer" (no hay camino entre ellas).
### En resumen:
El código simula explorar una red social para ver si dos personas están conectadas.
La función dfs explora la red a partir de una persona, siguiendo sus conexiones hasta llegar al objetivo.
La función main lee la información de la red y llama a dfs para determinar si las dos personas pueden conocerse.
