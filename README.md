# ConexLab

**ConexLab** es una aplicación web interactiva y didáctica diseñada para la visualización, exploración y cálculo paso a paso de **componentes conexas** y **matrices de caminos** en grafos no dirigidos. 

🔗 **Demostración en vivo:** [https://ivan-carrillo.github.io/ConexLab/](https://ivan-carrillo.github.io/ConexLab/)

---

## Características Principales

* **Generación Flexible de Grafos:** 
  * Modo **Al azar** con densidad controlada.
  * Modo **A mano** mediante simulación de matriz de adyacencia simétrica.
  * Ajuste de vértices dinámico ($5 \le |V| \le 15$).
* **Modelado Matemático e Interactivo:**
  * Cálculo dinámico de la **Matriz de Adyacencia ($A_1$)** con reflexividad en la diagonal.
  * Algoritmo de multiplicación booleana para la **Matriz de Caminos ($P$)**.
  * Reordenamiento matricial por bloques conexos.
* **Visualización de Grafos y Subgrafos:**
  * Dibujo vectorial interactivo en `<canvas>` HTML5.
  * Resaltado progresivo por colores para cada grupo conexo identificado.
  * Generación de subgrafos independientes por cada componente encontrada.
* **Enfoque Didáctico:**
  * Registro explicativo paso a paso (*Log*) para reforzar el aprendizaje de algoritmos sobre grafos.

---

## Tecnologías Utilizadas

* **HTML5:** Estructuración semántica de la interfaz y elementos Canvas.
* **CSS3 :** Diseño moderno estilo *Clean Academic Palette*, totalmente adaptativo (*responsive*).
* **JavaScript Vainilla:** Algoritmos de teoría de grafos, manipulaciones matriciales y renderizado 2D en tiempo real.
* **Google Fonts:** Tipografía *Nunito* para una legibilidad clara e instructiva.

---

## Modo de Uso

1. **Paso 1 · Configurar el Grafo:**
   * Selecciona el número deseado de vértices mediante el deslizador.
   * Elige entre generar una topología aleatoria o marcar las aristas manualmente en la matriz.
   * Haz clic en **Crear grafo**.
2. **Paso 2 · Iniciar Análisis:**
   * Presiona el botón **Calcular componentes**.
3. **Paso 3 · Explorar Resultados:**
   * Utiliza el botón **Siguiente paso** para observar de forma secuencial la identificación de cada grupo conexo.
   * Alternativamente, haz clic en **Mostrar todo** para desplegar de forma inmediata las matrices de adyacencia, caminos, bloques reordenados y la desintegración en subgrafos.

---

## Licencia y Créditos Académicos

Este proyecto fue desarrollado como trabajo del curso de **Matemática Computacional** en la **Universidad Peruana de Ciencias Aplicadas (UPCA / UPC)**.

* **Uso:** Estrictamente limitado a **fines académicos**, docentes y de investigación.
* **Autor:** Iván Carrillo & Equipo de Trabajo.