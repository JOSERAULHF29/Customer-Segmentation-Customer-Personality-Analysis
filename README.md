                                   Customer Segmentation – Customer Personality Analysis

Segmentación de clientes para diseñar estrategias de marketing personalizadas, utilizando análisis de datos y clustering.

Problema de negocio
-----------------------
Las empresas necesitan entender sus clientes para ofrecer productos y promociones que realmente se ajusten a su perfil.
El objetivo es segmentar clientes según:

.Ingresos
.Gasto total en productos
.Frecuencia de compra
.Comportamiento digital

y diseñar estrategias de marketing personalizadas para maximizar ventas y fidelización.

Metodología
------------------------
Selección de variables clave:

.Income (ingreso)
.total (gasto total)
.total_compras (frecuencia de compra)
.AGE (edad)

Normalización de datos:

Se aplicó StandardScaler para que todas las variables tengan la misma escala.
Determinación del número óptimo de clusters:
Se utilizó el Método del Codo basado en WCSS (Within-Cluster Sum of Squares).
Se eligieron 4 clusters, donde la reducción de WCSS empieza a estabilizarse.

Clustering con K-Means:
--------------------------
Cada cliente se asignó a un cluster según sus características.
Asignación de etiquetas descriptivas (Marketing):
Cada cluster se etiquetó con un nombre representativo:

.Bajo ingreso / Bajo gasto
.Clientes Premium
.Alto ingreso / Bajo gasto
.Clientes Jóvenes Digitales

Análisis descriptivo:
----------------------------
Se calculó el promedio de cada variable por cluster para entender el perfil de cada grupo.

| Categoría                  | Edad Promedio | Gasto Total Promedio | Compras Promedio | Ingreso Promedio |
| -------------------------- | ------------- | -------------------- | ---------------- | ---------------- |
| Bajo ingreso / Bajo gasto  | 48            | 118                  | 6                | 32,952           |
| Clientes Premium           | 69            | 1,149                | 19               | 69,858           |
| Alto ingreso / Bajo gasto  | 67            | 198                  | 8                | 43,267           |
| Clientes Jóvenes Digitales | 49            | 1,204                | 19               | 72,719           |


Interpretación:
------------------------------

.Clientes Premium: alto ingreso, alto gasto → estrategia: programas VIP
.Jóvenes Digitales: edad baja, alto gasto online → estrategia: campañas digitales
.Alto ingreso / Bajo gasto: clientes que podrían comprar más → estrategia: cross-selling / upselling
.Bajo ingreso / Bajo gasto: sensibles a precio → estrategia: promociones y descuentos


