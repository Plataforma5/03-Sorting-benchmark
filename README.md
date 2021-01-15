# Sorting Algorithm Benchmarking Demo

Una pequeña visualicación de sorting algorithims.

## Instalación

```sh
npm install # o yarn install
npm start # abre browser/index.html en tu browser
```

## Setup

**No estamos incluyendo las implementaciones** para bubble y merge sort en esto. Si corres el benchmarking asi como esta, los tres algoritmos son solamente los native sort. 

Abrir `browser > js > sorts.js` y reemplaza `bubbleSort` y `mergeSort` con tu propia implementación. Ahora refreshea la pagina de benchmarking.

## Calibrando

El visualizador genera arreglos random de largo basado en la potencia de dos. Por ejemplo con exponentes low y high  de 7 y 14, los arreglos van estar en el rango de 128 y 16,384. Eso pordría ser mucho para tu computadora para manejar! Podemos modificar estas constatntes en `browser/js/bench.js`.

## Algoritmos

Algoritmo | Promedio de time complexity | Peor caso en time complexity  | Peor Space Complexity | Notas
--- | --- | --- | --- | ---
Native (Quicksort) | O(n·log(n)) | O(n^2) | O(log(n)) | en practica / en promedio es bastante rapido
Merge Sort | O(n·log(n)) | O(n·log(n)) | O(n) | El peor caso es mejor q Quicksort
Bubble | O(n^2) | O(n^2) | O(1) | Simple, pero un time complexity terrible
