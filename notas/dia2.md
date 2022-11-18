Seguros de coche

AGE
GENDER
RACE
DRIVING_EXPERIENCE years
EDUCATION
INCOME
CREDIT_SCORE
VEHICLE_OWNERSHIP
VEHICLE_YEAR
MARRIED
CHILDREN
POSTAL_CODE
ANNUAL_MILEAGE
VEHICLE_TYPE
SPEEDING_VIOLATIONS
DUIS

OUTPUT .... Si el polluelo de turno ha tenido un accidente

Estimar la probabilidad de que una persona tenga un accidente. Para ver cuánto le cobro en el seguro!

El tener hijos afecta a tener un accidente: EN NADA !
El estar casado afecta a tener un accidente: EN NADA !
Los kilometros que hacen al año! En nada !

Afecta la altura a los conocimientos de matematicas? No, pero los datos dicen que si
Conocimientos de mates y altura en niños de 0 a 14 años SI HAY RELACION                 Relación espuría. Variable mediadora: EDAD!

Pregunta:
Sois una compañía de seguros.
Qué pensais que afecta a que una persona pueda tener mayor probabilidad de tener un accidente?
- Aspectos técnicos del vehículo
- Nivel de exposición al peligro
    POSTAL_CODE
    ANNUAL_MILEAGE                              A más kilometros más nivel de exposición al peligro ... más probabilidad de accidente
- De mi nivel de responsabilidad al volante
    EDAD
    MARRIED
    CHILDREN
    SPEEDING_VIOLATIONS 0 ... 15
                                        0 que pienso de él? Que nunca ha tenido multas por ser muy prudente o por qué no le ha dado tiempo !
                                        2 quizás tiene más responsabilidad... ya le ha visto las orejas al lobo!
                                        5 ---> CAFRE ! PERDIDO !
    DUIS
- Limitaciones físicas
- Nivel de concentración
    CHILDREN
    CREDIT_SCORE
- Mi experiencia como conductor
    EDAD
    ANNUAL_MILEAGE                              A más kilometros más experiencia... y por ende...        menos probabilidad de accidente
    DRIVING_EXPERIENCE


Learning! Aprender
Aprender. Es un proceso 1º de descarte de información

VARIABLE OBJETIVO (HECHO)  = f(FACTORES) < Variables

Técnica de reducción de dimensiones: PCA, Análisis factoriales

Tragsa -> Clara  (2 años)

Nivel de empoderamiento de una mujer
- Con la pasta
- Autoestima
- Con la capacidad de gestionar su tiempo
    Cuando comienza la semana, planifica usted las tareas que debe hacer a lo largo de la misma. --> Indefensión aprendida
- ..

8 factores - Test

------
Niños en el cole!
9 años

Les doy clase de mates.
 
Examen de mates! Les he enseñado a sumar y multiplicar!
¿cuál es el objetivo de ese examen? Evaluar conocimientos y ver si saben sumar y multiplicar?  No es el objetivo del examen.
                                    Ordenar a los niños en base a "sus conocimientos"
                                        Sobresaliente > Notable > Bien > Progresa adecuadamente

Variable
P1: 3 + 4               Estas preguntas guardan relación con la capacidad de sumar
P2: 7 + 8                               La comprensión del lenguaje, De la capacidad de concentración, de su reacción ante un examen: RUIDO !
-------------------------
P3: 7 x 9               Estas preguntas guardan relación con la capacidad de multiplicar
P4: 5 x 3
-------------------------
P5: 12 x 87              Estas preguntas guardan relación con la capacidad de multiplicar y sumar!

-------> Sumar los puntos: Técnica de reducción de dimensiones

Quizás puede ser que haya una pregunta muy mal expresada en el examen.


-----
# Estadística descriptiva

Conjunto de técnicas para resumir la información y hacerla más potable, entenderla mejor.

## Univariable

Me ayuda a entender el comportamiento de una población con respecto a una variable

### Tablas de frecuencias
### Estadísticos
#### Estadísticos de tendencia central:     POR DONDE VAN LOS TIROS !
    Moda            Nominal
    Mediana         Ordinal o Cuantitativa (distribución asimétrica)
    Media                     Cuantitativa (distribución simétrica)

#### Estadísticos de dispersión:            GROSO MODO, CUANTO CAMBIAN LAS COSAS CON RESPECTO AL "POR DONDE VAN LOS TIROS" !
    Desviación típica : Cuanto cambian las cosas con respecto a la MEDIA
    RSIC :              Cuanto cambian las cosas con respecto a la MEDIANA

### Gráficos:
  - barras     \
  - sectores   / tablas de frecuencias
  - histograma    variables cuantitativas

# Multivariable

Tratamos de identificar relaciones entre variables <<<<<< Esto lo bueno de verdad !

## Bivariables

Son cálculos sencillos, que puedo hacer a mano y entender.
Las técnicas que vamos a aplicar, para ver cuánta relación hay entre 2 variables dependen del nivel de medida de la variable

### Nominal x Nominal (1)

    Estadístico: ChiCuadrado, que tiene un problema: No tiene límite superior.. no lo puedo interpretar
                 V Crammer, Coef. Contingencia, Coef. Phi 0...1

### Nominal x Ordinal

    Si la variable Ordinal, la trato como Nominal, puedo hacer lo mismo que (1)
    Usando la información ordinal: Estudio de comparación de medianas. Para cada grupo (en base a la variable nominal) calculo la mediana
        Si las medianas de todos los grupos me dan el mismo valor? No hay relación

### Nominal x Cuantitativa

    Lo mismo que arriba
    Y además: Estudio de comparación de medias

### Ordinal x Ordinal

    Si uso de ambas su información nominal: Estudio chicuadrado y derivados
        > Hay mayor porcentaje de niños con paga ALTA de lo esperado . Identifica casillas sueltas de la tabla
    Si uso la información ordinal de la primera: Estudio de comparación de medianas (1) en función de los grupos que genere la (2)
        > Si hay grupos en función de una variable que tengan una mediana más alta que otros:
        > Los niños de mediana cobran más que los demás grupos
    Si uso la información ordinal de la segunda: Estudio de comparación de medianas (2) en función de los grupos que genere la (1)
    Si uso la información ordinal de ambas variables: R Spearman: -1 ... 1
        Miro el signo: 
            - Las variable guardan una relación INVERSA: Según sube una, baja la otra
            + Las variable guardan una relación DIRECTA: Según sube una, sube la otra
        > A más edad más paga 
            0: No hay nada de relación
            1: Hay una relación perfecta

### Ordinal x Cuantitativa
    Igual que el anterior...
    + Estudio de comparación de medias

### Cuantitativa x Cuantitativa
    Todos los anteriores 
    + Coeficiente de correlación de Pearson .... Se interpreta igual que el de Spearman: Su valor está entre -1 ... 1
        Si los puntos en un diagrama de dispersión están muy cerca o lejos de la recta de regresión de mínimos cuadrados 
        Miro el signo: 
            - Las variable guardan una relación INVERSA: Según sube una, baja la otra
            + Las variable guardan una relación DIRECTA: Según sube una, sube la otra
        Miro el valor absoluto: 
            0: No hay nada de relación
            1: Hay una relación perfecta
        

## Más de 2 variables

Son calculos complejos, que no puedo hacer a mano, ni muchas veces entender


----
Pagas que les damos a los niñ@s de 14 años a la semana

10 personas
SEXO        PAGA
1             10            10 12 12 14 20 = 68/5= 13.5
1             12
1             14
1             12 
1             20
2             14            14 20 16 18 10 = 78 / 5 = 15.6
2             20
2             16
2             18
2             10

   Mediana(Paga, hombres) = 12€
 - Mediana(Paga, mujeres) = 16€
  -----------------------------
                             4€ Los hombres, de mediana cobran de paga con 12 años 4 pavos menos que las mujeres.



   Media(Paga, hombres) = 13.5€
 - Media(Paga, mujeres) = 15.6€
                             De media los hombres cobran 2€ menos que las mujeres 
----
Ejemplo Spearman

Pagas que doy en función de la edad

Niño, Preadolescentes, Adolescentes, Jovenes
Nada , baja, alta, muy alta

Niño                Nada
Niño                Nada
Niño                alta
Preadolescente      nada
Preadolescente      baja
Preadolescente      baja
Adolescente         baja
Adolescente         alta
Adolescente         alta
Joven               alta
Joven               baja
Joven               muy alta


# Estudio Basado en la información nominal:

                        Nada    baja    alta    Muy alta
    Niño                 2       0        1         0
    Preadolescente       1       2        0 .       0           Chi cuadrado y derivados
    Adolescente          0       1        2         0               Esto sirve para identificar casillas que no encajan
    Joven                0       1        1         1

Usando la capacidad ordinal de la variable Edad:
    Mediana (edad, paga)
        Mediana (Nada): Niño                    Niño Niño Preadolescente
        Mediana (Baja): Preadolescente
        Mediana(alta):  adolescente
        MEdiana(muy alta): joven

Usando la capacidad ordinal de la variable Paga:
    Mediana (edad, paga)
        Mediana (Niño)              Nada
        Mediana (Preadolescente)    Baja
        Mediana(adolescente)        Alta
        MEdiana(joven)              Alta

Usando la información ordinal de las 2 variables
                                    Orden en función de Edad        Orden en función de la paga             RESTA (Diferencia)
Niño                Nada                2                               2                                     0
Niño                Nada                2                               2                                     0
Niño                alta                2                               9.5                                   7,5
Preadolescente      nada                5                               2                                     -3,5
Preadolescente      baja                5                               5.5
Preadolescente      baja                5                               5.5
Adolescente         baja                8                               5.5
Adolescente         alta                8                               9.5
Adolescente         alta                8                               9.5
Joven               alta                11                              9.5
Joven               baja                11                              5.5
Joven               muy alta            11                              12
                                                                                                                De aquí sale el Coef. Corr. Spearman



# Graficos

## Variable nominal u ordinal

Barra o sectores

## Variable cuantitativa

Histograma
Boxplot (caja y bigote)
Violin

## 2 variables: Nominales u ordinales

Barras apiladas
Barras paralelas

## 2 variables: Cuantitativa x (nominal u ordinal)

Pirámide poblacional (nominal es dicotómica)
Boxplot múltiple
Violín múltiple

## 2 variables cuantitativas

ScatterPlot (diagrama de dispersión)


---
# Boxplot

 ^ Variable
 |        
 |
 |      -----       "Máximo" de la variable
 |        |
 |        |
 |        |
 |      -----       Q3                      ^       Sumo del Q3 + 1.5xRIC
 |      |   |                               |
 |      +---+       Mediana = Q2            |       Altura de la caja: Q3-Q1 = RIC *1.5
 |      |   |                               |
 |      -----       Q1                      v       Resto del Q1 - 1.5xRIC
 |        |
 |        |
 |        |
 |        |
 |        |
 |        |
 |      -----       "Mínimo" de la variable
 |        
 |        o     Valores atípicos (gertrudis)
 |        o
 |
 |
 


----

2 variables cuantitativas: EDAD x ALTURA. 100 individuos entre 0 y 80 años

    ALTURA
    ^                    x|x x  xx x  xx x  xx x  xx x  xx x  xx x  xx x x  |
    |                     |xx x  xx x  xx x  xx x  xx x  xx x  xx x  xx x x | x  
    |                     |  xx x  xx x  xx x  xx x  xx x  xx x  xx x  xx x |x xxx x x  
    |                x  x |x                                                | xx xx xx x x 
 150|             x x     |                                                 |     xx x x 
    |           x x       |                                                 |
    |          x x        |                                                 |
    |        x x          |                                                 |
 100|      x x            |                                                 |
    |     x x   x         |                                                 |
    |     x xx            |                                                 |
    |   x x               |                                                 |
 40 |  xx x               |                                                 |
    |                     |                                                 |
    |                     |                                                 |
    |----------10---------|-20---------30----------40---------50---------60--------70-------80--> EDAD


# Lo de hacer predicciones, es algo que voy a hacer con frecuencia cuando analizo datos?

SIEMPRE HACEMOS PREDICCIONES ! Aunque creamos que no la estamos haciendo! 100% de los casos!

Imaginad que tenemos los datos de caída de nuestros servidores de aplicaciones de los últimos 5 años. No responden.
Y los analizo.

Estamos haciendo un estudio descriptivo o inferencial(predictivo)
- Listado de las caídas por meses del año:      Tabla de frecuencias de 2 variables
- Listado de las caídas por día de la semana
- La media de caídas al mes -> Voy a presuponer (predicción) que es la que sigo teniendo y la que voy a seguir teniendo

Aquí ya estoy haciendo una suposición enorme: Que el mundo va a seguir igual!

En estadística SIEMPRE suponemos que estamos trabajando con una MUESTRA de la POBLACION

----

Media de salario en ITNow

    ^ frecuencia
    |                                                       SIMETRIA: MUY SIMETRICO 
    |              XXXXXXXXX
    |         XXXXXXXXXXXXXXXXXX
    |        XXXXXXXXXXXXXXXXXXXXXX
    |     XXXXXXXXXXXXXXXXXXXXXXXXXXX 
    |   XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    ------------------------------------------> Salario

    |
    |                                                       SIMETRIA: MUY ASIMETRICA 
    |        XXXX
    |      XXXXXXXXXXX
    |     XXXXXXXXXXXXXXX                                   ESTO SI QUE VA A SER LA VARIABLE SALARIO
    |    XXXXXXXXXXXXXXXXXXXXXXXX 
    |   XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    ------------------------------------------> Salario


3000 nóminas de empleados (todos los empleados reales que tiene hoy en día ITNOW)..... quiero la media.

En cada curso voy a preguntar a la peña cuantos billetones ganan.
16 compañeros           6800 7200 5400 9200 5490 ......     6000€ / mes MEDIA DE QUE ? una muestra = Media real de ITNOW(población)
Ahora... no tengo el dato real.. solo este. ¿Puedo decir que la media real de la población (todos los empleados) se aproxima a este valor?
-------
Voy a un parque: Y hay gente... y les pregunto, cuanta pasta ganais:
1000 1000 1000 1000 1100 1000 980 1000 1050 1000 1000     x?       Media: 1020€
    - Cuanto de vuestro sueldo os jugais a que la persona gana 1020€?   En general os jugais POCO
                                                                        Cada uno de vosotros teneis vuestro propio nivel de riesgo

    - Cuanto de vuestro sueldo os jugais a que la persona gana entre 800-1200€?   Más que antes
    - Cuanto de vuestro sueldo os jugais a que la persona gana entre 500-1500€?   Más que antes
    - Cuanto de vuestro sueldo os jugais a que la persona gana entre 0-1500000€?  El sueldo, los niños, el coche!

Siempre existe probabilidad de cagarla... Según aumento el interval: BAJA

He preguntado solo a 10 personas en el caso anterior.....
Pero ahora... me esmero y pregunto a 20000 personas en el parque, durante sucesivos días.... y todas me dan ese tipo de valores
Esto me haría jugarmela más o menos? MAS ... Detecto que hay menos probabilidad de cagarla

La gente a la que pregunto me dice esto:
1000 2000 3000 0 500 10000 750 6000 1050 100000 0     x? 
Esto me haría jugarmela más o menos? MENOS . Detecto que hay más probabilidad de cagarla


A la hora de hacer una predicción y de establecer un rango de confianza, hay cosas que nos afecta a la probabilidad de cagarla:
- La dispersión de los datos. No hay manera de trucar esto! no es manipulable
- La cantidad de gente de la que tengo datos. Puedo jugar aquí?  PUEDO PREGUNTAR A MAS GENTE ----> bajo la probabilidad de cagarla

Aumentar el intervalo de confianza -----> bajo la probabilidad de cagarla!

-----
TEOREMA DEL LIMITE central

Si tomamos todos los potenciales grupos (muestras) de un determinado tamaño n, de una población de tamaño N,
La medias de cada muestra siguen una distribución NORMAL, con total independencia de cómo sea la población original.
Normal, de media la misma que la de la variable original
       y de desviación típica, la de la variable original dividido entre raiz(n)


    
    | POBLACION los individuos y su salario
    |
    |         XXXX                                              MEDIA = 1500€
    |      XXXXXXXXX|XX                                         DESV. TIPICA = 400€
    |     XXXXXXXXXX|XXXXX
    |    XXXXXXXXXXX|XXXXXXXXXXXXX 
    |   XXXXXXXXXXXX|XXXXXXXXXXXXXXXXXXXXXXXX                                36  + 24 + 15 + 11 + 4 = 90 = N
    ----500---1000--^-1500-----2000------2500-------------------> Salario
                ^   MEDIANA
               MODA     ^
                        MEDIA

    | POBLACION: Las muestras y sus medias
    |
    |                  XXX                                         
    |                XXXXXXX                                       MEDIA = 1500
    |              XXXXXXXXXXX                                     DESV. TIPICA = 400€ / RAIZ(n)
    |   2,5%    XXXXXXXXXXXXXXXOXX      2.5%
    |     xxX|XXXXXXXXXXXXXXXXXXXXXX|Xxx                             
    ----500--a1000---1500-----2000--b---2500-------------------> Salario
                       ^
                      MEDIA

Muestra n = 100 : INFINITAS muestras
                            MEDIA
Muestra 1                   1500
Muestra 2                   2000
Muestra 1000000              600
Muestra INFINITAS

Pido (usando las integrales que han dado los matemáticos), que se calcule a y b, tal que dejen fuera un 5% de las muestras potenciales.
Las más raras fuera!
Me la juego a que la muestra que yo he cogido. Probabilidad de cagarla: 5% - 1 de cada 20

Cuando distará como mucho esa muestra de la media real? (b-a)/2 -> Intervalo de confianza! Para un 5% (b-a)/2= 1.96 x desv.tipica (400/RAIZ(n)) = 80

    Si el salario de la media que yo he calculado está en 1650€ + - 80... hay tengo un 95% de confianza en que está la media real!

Alturas de personas de 40 años


                   XXXX                   XXX
                XXXXXXXXXX              XXXXXXX
              XXXXXXXXXXXXXXXXXX      XXXXXXXXXXX
            XXXXXXXXXXXXXXXXXXXXX   XXXXXXXXXXXXXXXX
        XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
---------------------^----------------------^----------------------
                    160                    170


Cualquier media que mida (que será por definición siempre en una muestra) le puedo pedir a los programas informáticos(librerias de python) que me calculen
El intervalo de confianza al 95% (o cualquier otro valor): 80
De forma que tendré una confianza del 95% en que la media real estará entre la que he encontrado y 1 intervalo de confianza por arriba o abajo



Medimos las caidas del mes de marzo y de abril de los servidores

Marzo: Media 20 caidas          + 5         = 15-25
Abril una media de 24 caidas.   + 4         = 20-28

Puedo concluir que en abril hay más caidas que en marzo?

Esta medida (el intervalo de confianza) lo que habla es de CUANTO CONFIO YO en los datos que tengo!
Esto depende de:
- la cantidad de datos
- de la desviación típica (dispersión) ... No es manipulable

La pregunta va a ser, al crear un modelo, tengo suficientes datos, como para poder sacar conclusiones / hacer predicciones?

n = 10.000.000
 g1 = 5.000.000
 g11 = 10.000
 edad = Jovenes = 2.000
    Interés: Play: 250