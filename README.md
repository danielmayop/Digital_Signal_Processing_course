# Procesamiento Digital de Señales (imágenes)

Este curso de procesamiento digital de señales tomó los siguientes temas para desarrollar este trabajo práctico.

Cada trabajo práctico (TP) está resuelto en un notebook de Jupyter y aplica en Python los conceptos vistos en las clases teóricas.

## Temas del curso

Las diapositivas de teoría están en la carpeta [`Teoria/`](Teoria/):

- Espacios cromáticos
- Aritmética de píxeles
- Operaciones de luminancia
- Transformada de Fourier
- Procesamiento por convolución
- Procesamiento morfológico
- Remuestreo, reconstrucción, cuantización y compresión
- Segmentación
- Representación y descripción

## Trabajos prácticos

| TP | Notebook | Tema | Qué se hace |
|----|----------|------|-------------|
| 1 | [`PDI_tp1.ipynb`](PDI_tp1.ipynb) | Espacios cromáticos | Separación de una imagen en sus canales RGB, conversión RGB ↔ YIQ y modificación de los componentes de luminancia y color. |
| 2 | [`PDI_tp2.ipynb`](PDI_tp2.ipynb) | Aritmética de píxeles | Suma y resta de imágenes (clampeada y promediada), interpolación entre dos imágenes y operaciones "if lighter" / "if darker". |
| 3 | [`PDI_tp3.ipynb`](PDI_tp3.ipynb) | Operaciones de luminancia | Histogramas, clamping, función lineal a trozos y funciones raíz, cuadrado y potencia aplicadas sobre la luminancia. |
| 4 | [`PDI_tp4.ipynb`](PDI_tp4.ipynb) | Transformada de Fourier | Cálculo de módulo y fase, antitransformada y eliminación de patrones indeseados (como las barandas de un puente) modificando el módulo. |
| 5 | [`PDI_tp5.ipynb`](PDI_tp5.ipynb) | Procesamiento por convolución | Filtros pasa bajos (kernel plano, Bartlett y gaussiano), pasa banda y pasa altos, y detectores de bordes (Laplaciano de vecindad 4 y 8, Sobel). |
| 6 | [`PDI_tp6.ipynb`](PDI_tp6.ipynb) | Procesamiento morfológico | Dilatación, erosión, apertura, cierre, borde interno y externo, mediana y top hat con distintos elementos estructurantes. |
| 7 | [`PDI_tp7.ipynb`](PDI_tp7.ipynb) | Remuestreo | Reducción (downsampling, también con promedio) y ampliación (upsampling) de imágenes. |

## Herramientas

Los notebooks usan Python con [OpenCV](https://opencv.org/), [NumPy](https://numpy.org/) y [Matplotlib](https://matplotlib.org/). El TP 7 también usa [SciPy](https://scipy.org/).

## Cómo ejecutarlos

1. Instalar las dependencias:

   ```bash
   pip install opencv-python numpy matplotlib scipy jupyter
   ```

2. Abrir el notebook que se quiera ver:

   ```bash
   jupyter notebook PDI_tp1.ipynb
   ```

Algunos notebooks cargan imágenes propias (por ejemplo `mi_img.jpg` en el TP 1), así que hay que ubicar las imágenes en la ruta que indica cada notebook antes de ejecutarlo.
