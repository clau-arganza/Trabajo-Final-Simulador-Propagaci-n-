# Simulador de Propagación de Información en Redes Sociales

Este proyecto se ejecuta en un **Jupyter Notebook** y simula cómo se propaga la información (por ejemplo, un rumor) a través de una red social representada mediante un grafo no dirigido.

# Instrucciones para Ejecutarlo

1. Asegúrate de tener instalado Jupyter Notebook.
2. Instala las bibliotecas necesarias ejecutando en tu terminal:

```bash
pip install networkx matplotlib numpy
```

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
