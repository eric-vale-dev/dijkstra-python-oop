# 🗺️ Dijkstra's Algorithm with Custom Min-Heap

Este repositorio contiene una implementación robusta en **Python** del algoritmo de Dijkstra para encontrar las rutas más cortas en un grafo. Este proyecto fue desarrollado como práctica para la materia de Análisis y Diseño de Algoritmos.

## 📌 Propósito del Proyecto
El objetivo principal es calcular la distancia mínima desde un nodo origen (source) hacia todos los demás vértices de un grafo ponderado. 

Lo que hace especial a esta implementación es que **no utiliza librerías estándar** para el manejo de la cola de prioridad. En su lugar, incluye una clase personalizada (`min_heap_pq`) construida desde cero que gestiona las operaciones de un **Min-Heap**, demostrando un profundo entendimiento de las estructuras de datos fundamentales.

## ✨ Características Técnicas
* **Programación Orientada a Objetos (OOP):** El código está estructurado en clases claras (`min_heap_pq` para la estructura de datos y `Dijkstra` para la lógica del algoritmo).
* **Custom Min-Heap:** Implementación manual de funciones críticas como `min_heapify`, `extract_min`, `decrease_key` y `min_heap_insert`.
* **Unique Shortest Path (USP):** El algoritmo no solo calcula la distancia, sino que también determina si el camino más corto encontrado hacia un nodo es único (1) o si existen múltiples caminos con el mismo peso mínimo (0).
* **Grafos No Dirigidos:** Lógica adaptada para evaluar aristas bidireccionales de forma eficiente.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python 3
* **Conceptos:** Grafos, Estructuras de Datos (Heaps/Colas de Prioridad), Algoritmos Voraces (Greedy).

## 🚀 Cómo ejecutar el proyecto
Si estás en un entorno Linux (como Fedora, Ubuntu) o macOS, abre tu terminal y ejecuta los siguientes comandos:

1.  Clona este repositorio y navega a la carpeta del proyecto.
2.  Ejecuta el script con Python 3:
    ```bash
    python3 Dijkstra.py
    ```

### Ejemplo de Salida Esperada
El código incluye un bloque de prueba (`if __name__ == "__main__":`) con un grafo de 5 nodos preconfigurado. Al ejecutarlo, verás en consola un resultado similar a este:

```text
El algoritmo ha terminado.
Formato del resultado: [distancia_minima, unique_shortest_path]
Hacia el vértice 1: [0, 1]
Hacia el vértice 2: [2, 1]
Hacia el vértice 3: [3, 1]
Hacia el vértice 4: [9, 1]
Hacia el vértice 5: [6, 1]