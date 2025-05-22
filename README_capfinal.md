# Simulador de Propagación de Información en Redes Sociales

Este proyecto se ejecuta en un **Jupyter Notebook** y simula cómo se propaga la información (por ejemplo, un rumor) a través de una red social representada mediante un grafo no dirigido.

# Instrucciones para Ejecutarlo

1. Asegúrate de tener instalado Jupyter Notebook.
2. Instala las bibliotecas necesarias ejecutando en la primera celda:

!pip install networkx matplotlib numpy

3. Abre el archivo `ejercicio_cap.ipynb` en Jupyter Notebook.
4. Ejecuta las celdas una por una para:
   - Generar la red social.
   - Calcular los caminos más cortos entre los nodos usando el algoritmo de Floyd-Warshall.
   - Simular la propagación de la información.
   - Visualizar la propagación paso a paso.

# Bibliotecas utilizadas

- `networkx`: para modelar y manipular grafos.
- `matplotlib`: para crear visualizaciones gráficas.
- `numpy`: para manejar operaciones numéricas y matrices.

# Qué hace el simulador

Cada nodo representa una persona, y cada arista una relación directa (amistad, seguimiento, etc.). Se calcula cuánto tiempo tarda la información en llegar a cada nodo desde una fuente inicial, y se visualiza el proceso de propagación en la red.

El algoritmo de Floyd-Warshall encuentra los caminos más cortos entre todos los pares de nodos, lo que permite modelar la propagación de forma precisa considerando la estructura global del grafo.

Este proyecto es útil para analizar cómo se difunden noticias, rumores o ideas en redes sociales reales.

# Parámetros de entrada del simulador

Al ejecutar la siguiente celda, el simulador solicitará tres entradas por teclado:

1. **Número de personas**: un número entero que representa la cantidad de nodos (usuarios) en la red social.
2. **Probabilidad de conexión**: un valor decimal entre 0 y 1 que indica la probabilidad de que exista una conexión entre dos personas.
3. **Nodo de inicio del rumor**: un número entero entre 0 y n-1 que representa el nodo desde el cual comenzará la propagación de la información.

Estas entradas permiten personalizar la simulación de acuerdo al tamaño de la red y su conectividad.

# Casos extremos a considerar:

- **Probabilidad = 0**: Ninguna persona está conectada con otra. El rumor no se extenderá más allá del nodo de inicio.
- **Probabilidad = 1**: Todas las personas están conectadas con todas. El rumor se propaga de forma instantánea a toda la red.

Estos escenarios ayudan a comprender cómo la estructura de la red influye en la velocidad y alcance de la propagación.

