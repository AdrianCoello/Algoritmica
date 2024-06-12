## Explicación del código de búsqueda en anchura (BFS)

**Descripción general:**

El código implementa la búsqueda en anchura (BFS) para determinar si un nodo (persona) puede llegar a otro en una red social (grafo). 
La BFS explora la red a partir de una persona (nodo inicial), visitando a todos sus vecinos (personas conectadas) antes de pasar a los 
vecinos de los vecinos, y así sucesivamente. Si la BFS marca el nodo final como visitado, significa que la persona inicial sí puede 
conocer a la persona final. El código utiliza una cola para ir explorando los nodos nivel por nivel, como si fuera una fila de personas 
esperando ser atendidas.

## Partes relevantes del código BFS:

**1. Función bfs:**

- **Toma un nodoInicial como parámetro.**
- **Utiliza una cola para almacenar los nodos a explorar.**
- **Agrega el nodoInicial a la cola y establece su nivel a 0.**
- **Mientras la cola no esté vacía:**
- **Obtiene el nodoActual de la cola.**
- **Si el nodoActual no ha sido visitado:**
- **Lo marca como visitado.**
- **Recorre sus vecinos:**
- **Para cada vecino:**
- **Calcula su nivel como el nivel del nodoActual más 1.**
- **Si el vecino no ha sido visitado:**
- **Lo agrega a la cola.**

**2. Función main:**

- **Lee el número de nodos y aristas de la red social.**
- **Lee las aristas y las almacena en la estructura grafo.**
- **Lee los nodos inicial (S) y final (T).**
- **Llama a la función bfs con el nodo inicial S.**
- **Si el nodo final T está marcado como visitado, imprime "Si lo podria conocer".**
- **De lo contrario, imprime "No lo podria conocer".**

**En resumen:**

- La función bfs explora la red nivel por nivel, visitando a todos los nodos de un nivel antes de pasar al siguiente.
- La función main lee la información de la red y llama a bfs para determinar si las dos personas pueden conocerse.
