# BeesDataset
Set de datos utilizado para el proyecto de diagnóstico de colmenas de abejas mediante el análisis del sonido emitido con redes neuronales convolucionales o CNN.

# Método
Los datos fueron obtenidos en distintas colmenas de la Región Metropolitana y la Región de Valparaíso bajo las clasificaciones de "Healthy" (colmena sana) y "Sick" (colmena anómala o que presenta alguna enfermedad) con la ayuda de un veterinario especialista en sanidad apícola. La captura del audio de las colmenas de abejas se realizó con un micrófono Rode NTG-2 y una interfaz Behringer UMC-202 HD. Luego estos registros de audio fueron preprocesados y segmentados en muestras de cinco segundos. Finalmente cada muestra se transformó en un espectrograma en formato .png.

# Contenido
El set de datos contiene 8.155 datos en formato de imágenes separados en las clases "Healthy" y "Sick", de los cuales 3.815 son espectrogramas de colmenas sanas y 4.358 son espectrogramas de colmenas anómalas.

# Modelo
El modelo implementado con el cual fueron utilizados los datos es el modelo VGG16, cuya implementación se reentrenó mediante el método de Transfer Learning. Los resultados de este modelo logran predecir la clase a la que pertenecen con un 94% de precisión.
