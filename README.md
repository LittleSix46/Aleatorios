# Aleatorios
Repositorio de Debugging Aleatorios

Se puede observar que el programa no funciona como deberia

https://github.com/LittleSix46/Aleatorios/assets/163340762/972c7fe1-369d-45d7-9562-22ad69fdf32f

Despues de poner un punto de ruptura en la linea 10 y al pasar entre la 10 y 11 podemos observar que el valor de la variable siempre es un numero decimal menor a 1 por lo tanto al estar definido como (int) se acorta a 0 y despues de multiplicar por 100 se queda en 0
![image](https://github.com/LittleSix46/Aleatorios/assets/163340762/84d254a5-d5f0-42f6-8d9c-6d8fef9c02db)

Para corregir este problema simplemente cambiamos en la linea 11 el codigo

num_aleat[i] = (int)Math.random()*100; por num_aleat[i] = (int)(Math.random()*100);

Despues de hacer este cambio podemos observar que ahora el programa si funciona de manera correcta generando la cantidad de numeros aleatorios deseados.

https://github.com/LittleSix46/Aleatorios/assets/163340762/7ed6666a-772b-4c6d-b22b-09d81f54a2aa

