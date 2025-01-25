# Simulacion Compra Ecommerce

Este proyecto aborda la optimización de las entregas de productos en un comercio de Ecommerce. Se utilizó una simulación de Montecarlo para modelar la incertidumbre en las ventas y pedidos de los clientes, lo que permitió generar escenarios de demanda. Posteriormente, se formuló un problema de programación lineal para optimizar las entregas de los productos, utilizando los algoritmos Greedy y Greedy Aleatorio para encontrar soluciones aproximadas a este problema.

## Metodología
El proceso de este proyecto se llevó a cabo en las siguientes etapas:

### 1. Simulación de Montecarlo
Se utilizó la simulación de Montecarlo para modelar el comportamiento estocástico de las ventas y pedidos de compra de los productos en el ecommerce. Los pasos incluyen:

- Recopilación de Datos Históricos: Se utilizó un conjunto de datos históricos sobre las ventas de productos y los pedidos de compra de los clientes. Estos datos incluyen información como el número de productos vendidos por día, los tipos de productos más populares.

- Simulación de la Demanda: Mediante el uso de Montecarlo, se generaron varios escenarios de ventas y pedidos de productos, basados en las frecuencia de compra de los datos históricos. Esto permitió crear una variedad de posibles escenarios para evaluar la eficiencia de los modelos de optimización de entregas en diferentes situaciones.

### 2. Formulación del Problema de Programación Lineal
El siguiente paso consistió en la formulación de un problema de programación lineal (PL) para optimizar el proceso de entrega de productos. El problema se formuló con el objetivo de minimizar los costos de entrega, considerando factores como:

- Capacidad de los vehículos de entrega: Cuántos productos pueden ser entregados en cada viaje.
- Restricciones de tiempo y espacio: Limitaciones relacionadas con la disponibilidad de los vehículos y la cantidad de productos a entregar.
Se definieron las variables de decisión, la función objetivo y las restricciones del modelo de programación lineal, permitiendo calcular el número óptimo de entregas y rutas a seguir para satisfacer la demanda de los clientes de la manera más eficiente.

### 3. Solución del Problema con Algoritmos Greedy
Una vez formulado el problema de programación lineal, se implementaron dos enfoques heurísticos para resolverlo:

- 3.1 Greedy (Codicioso)
El algoritmo Greedy sigue la estrategia de tomar las decisiones más beneficiosas de manera local en cada paso. Para el problema de entrega de productos, el algoritmo selecciona iterativamente el pedido más cercano o el más prioritario hasta que todos los pedidos se hayan asignado a entregas.

- 3.2 Greedy Aleatorio
El Greedy Aleatorio es una variante del algoritmo Greedy que introduce un componente de aleatoriedad en la toma de decisiones. En lugar de tomar siempre la decisión óptima localmente, en algunos casos se seleccionan decisiones al azar dentro de un conjunto de opciones cercanas. Esto permite explorar diferentes soluciones y, potencialmente, encontrar rutas más variadas y menos propensas a quedar atrapadas en soluciones subóptimas.
