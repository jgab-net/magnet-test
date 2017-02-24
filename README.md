# magnet-test

## Test

+ Se espera que al presionar cada uno de los botones que se muestran al abrir el archivo "index.html" 
    se muestre un alert indicando el número del botón que se presionó, 
    sin embargo, muestran un mensaje erróneo.
+ Solucionar el problema editando solamente el archivo "main.js"


## Solución 

Cuando se ejecuta el evento onclick el entorno en el que se creo la función se pierde, es decir, i tiene el ultimo 
valor que obtuvo, para solucionar esto usamos un closure, este guarda el entorno en el que se crea la función para
el evento onclick, guardando el valor de i en un scope para cada onclick. 