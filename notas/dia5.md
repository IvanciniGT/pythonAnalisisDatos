# Modelización - Machine learning

Me interesa darle a la computadora cuantas menos variables mejor:
- Los cálculos son muy complejos.. y cuantás más variables, más complejos
- Los fenómenos en la naturaleza normalmente no dependen de tantos factores, por lo menos la tendencia general.
- Por que la computadora al final va a generar una ecuación matemática. 
    Esta me interesa en la medida de lo posible entenderla / ser capaz de explicarla (ES UN REQUISITO LEGAL)

En general nos interesa (para cierto tipo de modelos) dar una explicación, y eso implica entender los factores 
que estoy teniendo en cuenta, entender que son esas variables que meto en el modelo.

    Variables       Factores                             Fenomeno a predecir
    Casado      \
    Hijos        > Responsabilidad de la persona        > Si se da la ostia
    Bebe mucho  /

Además, me interesa entender el modelo, para ver si tiene sentido, 
y por tanto es un modelo que vaya a funcionar en el grueso de los casos.

-----

Una vez tenga esos factores, montaré un modelo. ¿Cómo se hace eso?

Coleccion de datos pasados (histórico)  Variable / fenómeno a predecir : Y: Variable dependiente
                                        Un montón de datos que he recabado X -> Factores
                                        
        X1  X2  X3  ... Xn  ->  F1  F2  ... Fm -> Y         F1      F2          Y
Lucia   30 años, 5 hijos, 120 glucosa, 200 insulina.... -> 33       187     ->  No es diabética = 0
Pepita  30 años, 5 hijos, 120 glucosa, 200 insulina.... -> 20       287     ->  Si es diabética = 1
Marta   30 años, 5 hijos, 120 glucosa, 200 insulina.... -> 10        87     ->  No es diabética = 0
.....
Tropemil

* NOTA: Con m mucho más pequeño de n
    
    a*F1 + b*F2 =  Y lo que debería dar
    
    a*33 + b*187 = 0.1 -> 0.     0            √
    a*20 + b*287 = 0.7 -> 1      1            √
    a*10 + b*87  = 0.6 -> 1      0            x       Con esos valores, tengo un éxito del 66%

    Iteración 1: Prueba con a=2 ,b=-18
    Iteración 2: Prueba con a=2.1 ,b=-18.1

    El ordenador se pone a probar "aletaoriamente" valores de a y b , sobre todas las ecuaciones... y calculando un resultado

tropemil ecuaciones... con cuantas incógnitas? 2

El gran problema del mundo de la modelización: SOBREAJUSTE / RECALENTADO


Si tengo 100.000 datos, no los uso todos para calcular el modelo.
Solo uso una parte: 75%. Aplico el modelo para ese 75%. 
    Me sive ta tasa de éxito que obtenga aquí para evaluar la calidad del modelo? NO 
La prueba de fuego la haré con el 25% de los datos que han quedado. Los que no han influido para calcular el modelo.

En ocasiones partimos los datos en 3 grupos:
- D1 Los datos que voy a usar para crear 10 modelos.
- D2 Datos que voy a usar para ver qué modelo da mejor resultado, tiene más calidad.
- D3 Datos para obtener una medida de la calidad del modelo

Modelo, La calidad del modelo, la confianza en el modelo (significación)

Intentamos del grueso de datos, sacar muestras REPRESENTATIVAS para crear el modelo y para probarlo.


Como medida de la calidad del modelo: Su tasa de éxito... tenemos el charco que os conté ayer!


    
Las computadoras representan un número decimal: COMA FLOTANTE
    MANTISA(tamaño) EXPONENTE
                                Mantisa de 8
    0.00000000000012345678      12345678 x 10^(-20)
    12345678,123                                    Aquí no entran los dígitos significativos en la mantisa

Los datos de entrada, suelen venir en distintas unidades:
    Edad: 0-100
    Pedigree: 0-2
    Recuento de globulos blancos: Millones

Qué me puede interesar hacer con los datos, antes de trabajar: UNIFICAR, hacer un gradiente común:
Minimo y máximo sean "iguales" entre las variables.


Normalmente lo que hacemos cuando vamos a meter variables en un modelo es meter sus valores TIPICOS o NORMALIZADOS
Puntuación Z

|
|
|
|
|                                   XXXXXXXXX
|                                XXXXXXXXXXXXXXX
|                           XXXXXXXXXXXXXXXXXXXXXXXXX
|                        XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
|-----------------^--------------< -----^----- >----------------------------
                  0                    100

|
|
|
|
|             XXXXXXXXX
|          XXXXXXXXXXXXXXX
|      XXXXXXXXXXXXXXXXXXXXXXXXX
|   XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
|-----------------^---------------------^---------------------------------
                  0                    100


P1 = 3+5
P2 = 7+7
P3 = 3*9
P4 = 7*1

El chaval ha saco un 3.. PERO DONDE FAALLA !!!

Sumar                  0.05xP1 + 1xP2
Felipin:                    1
    P1 = 1
    P2 = 0
Marcial:                    1
    P1 = 1
    P2 = 0
Lucas:                      2
    P1 = 1
    P2 = 1
Rubiales                    0
    P1 = 0
    P2 = 0
    
    Porcentaje deacierto / No acierto
        Pregunta 50% acierta y 50% fallan... Es muy discriminadora
        Pregunta 10% aciertan es iguyal de poco valiosa que una donde solo el 10% fallan
    
Si miro las otras 800 personas que han hecho el examen
799 han fallado en la P2. EL PROFE ES UN CABRON !!!! Y ha puesto una pregunta que no cuela !!!


Multiplicacion
P3 = 1
P4 = 1