# Analizando tubos de ensayo

En un enorme laboratorio de análisis clínicos se deben analizar `n` muestras de sangre de numerosos pacientes.

Cada muestra está contenida en un tubo de ensayo.

Los tubos se encuentran ubicados en una enorme gradilla circular giratoria con exactamente `n` posiciones donde ubicar los tubos.

Esta gradilla se controla mediante dos botones. Cada botón permite rotar la gradilla en exactamente una posición, de modo que cada tubo quede ubicado en donde estaba su vecino correspondiente.
Uno de los botones permite girar en sentido horario, y el otro en sentido antihorario.

Por fuera de la gradilla, frente a cada una de las `n` posiciones donde están los tubos, se encuentran estacionadas máquinas de análisis. Las distintas máquinas no son todas iguales: algunas pueden realizar tipos de análisis que otras no.

Por cada una de las `n` muestras, se conoce un listado que indica cuáles de las n máquinas son capaces de analizarla.

El tiempo de análisis de una muestra es despreciable, y se pueden estar analizando varias muestras al mismo tiempo (necesariamente en distintas máquinas), pero el tiempo de rotación de la máquina es sumamente lento.

Por esta razón, tu tarea consiste en calcular la mínima cantidad de pulsaciones de botón que es necesario utilizar para que todas las muestras sean analizadas por alguna máquina.
Las muestras se numeran de 0 a n−1 en sentido horario, al igual que las máquinas analizadoras. Inicialmente, la máquina `i` se encuentra frente al tubo `i`.

### Objetivo

- Debes implementar la función: `tubitos(muestras)`
  - muestras: arreglo de n cadenas de caracteres, cada una formada por exactamente `n` caracteres S o N. Si el caracter `j` de `muestras[i]` es S, significa que la máquina `j` Sí puede analizar la muestra `i`, y si es N significa que la máquina `j` No puede analizar la muestra `i`.
  - Debe retornar un entero: la mínima cantidad de pulsaciones de botón necesarias para poder analizar todas las muestras.
  - Cotas 2 ≤ n ≤ 300 Todas las cadenas de texto contienen como mínimo una S.
