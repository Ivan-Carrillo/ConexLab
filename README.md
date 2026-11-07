# ConexLab

Aplicación web para determinar las **componentes conexas** de un grafo no dirigido a partir de su matriz de adyacencia booleana. Muestra el cálculo paso a paso, desde la matriz de caminos hasta la separación del grafo en subgrafos.

**Demostración:** https://ivan-carrillo.github.io/ConexLab/

---

## Características

- **Creación de grafos**
  - *Al azar:* genera una matriz simétrica con cada arista presente con probabilidad 0,2.
  - *A mano:* permite marcar las aristas en una tabla. Cada casilla se refleja automáticamente en su simétrica, así que la matriz siempre es válida para un grafo no dirigido.
  - Número de vértices ajustable entre 5 y 15. Al cambiarlo, la tabla conserva las aristas ya marcadas que sigan dentro del nuevo tamaño.
- **Identificación de estaciones:** cada vértice tiene una inicial fija (por ejemplo, CE, AB, AN). Solo se muestran las iniciales de los vértices elegidos, junto con una leyenda con el nombre de cada uno.
- **Cálculo matemático**
  - Matriz de adyacencia con 1 en la diagonal.
  - Matriz de caminos mediante la suma de potencias booleanas hasta la potencia *n − 1*.
  - Agrupación de los vértices por filas, con la matriz reordenada en bloques.
- **Visualización**
  - Grafo asociado dibujado en un lienzo HTML5, con cada grupo en un color distinto.
  - Subgrafo independiente para cada componente encontrada.
- **Registro explicativo:** cada paso del recorrido se acumula en una lista para seguir el razonamiento de principio a fin.

## Uso

1. **Configurar el grafo**
   - Elige el número de vértices con el deslizador.
   - Presiona **Al azar** para generar un grafo aleatorio, o **A mano** para marcar las aristas en la tabla.
2. **Calcular**
   - Presiona **Calcular componentes**. Aparecerán las matrices de adyacencia y de caminos.
3. **Explorar el resultado**
   - **Siguiente paso** muestra un grupo a la vez, con su explicación.
   - **Mostrar todo** completa el recorrido de inmediato.
   - **Empezar de nuevo** reinicia la aplicación.

## Estructura del repositorio

```
ConexLab/
├── index.html   # Aplicación completa (HTML, CSS y JavaScript)
├── README.md    # Este documento
```

## Ejecución local

No requiere instalación. Descarga el repositorio y abre `index.html` en su navegador de preferencia.

## Limitaciones

- Solo trabaja con grafos no dirigidos.
- Usa el método matricial del curso.
- Las iniciales están fijas para 15 estaciones; cambiarlas requiere editar el código.

## Créditos y licencia

Proyecto desarrollado por estudiantes de la **Universidad Peruana de Ciencias Aplicadas (UPC)** como trabajo del curso **1AMA0475 Matemática Computacional**

Uso restringido a **fines académicos**: estudio, enseñanza y evaluación.