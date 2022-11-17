
# Estadística?

Es una ciencia (independiente de las matemáticas) que estudia qué? Poblaciones 
En contraposición con otras ciencias, que se centran en el estudio de casos / individuos.

RRHH deITNow
- No me interesa saber lo que gana una persona
- Me interesa saber, por donde van los tiros en ITNOW
- Comparar empresas
- PREDECIR mi sueldo en ITNOW ! NUNCA HAY CERTEZA !!!
  - Posos del Té/Café                   \
  - Bolita de cristal                    > No son científicas... No son capaces de 
  - Consultar a Rapel / Carlos Jesús    /      TASAR la PROBABILIDAD DE CAGARLA

## Estadística descriptiva 

El conjunto de técnicas que nos ayudan a:
- resumir información 
- Presentar esa información
para hacerla más potable. Que sea capaz de entenderla.

### Univariable
### Multivariable
#### Bivariables / Tres variables 
#### Cuando tengo más de 3/4 variables, necesito aplicar técnicas de Machine Learning o Data mining

## Estadística Inferencial = Estadística descriptiva + Teoría de Probabilidad

Quiero aplicar la información(conocimiento extraído de la población) de la población
para PREDECIR casos concretos; pudiendo obtener una medida de la probabilidad de CARGARLA.

## Comentarios acerca de la estadística

- A veces puede ser engañoso
- El papel lo aguanta todo

Cuidado:
- Nunca puedo perder de vista que vamos a hacer PREDICCIONES, sujetas a error.
- Hay que saber aplicar las técnicas.

# Business Intelligence

El cómo aplicar técnicas estadísticas "simplonas" a datos de una empresa para 
ayudarme a tomar decisiones "evidentes" a futuro.

# Data mining

Conjunto de técnicas (estadística + matemáticas + Ciencias de la computación)
para identificar patrones ocultos en conjuntos de datos.
No tengo ni idea de lo que busco!

# Machine learning - Aprendizaje automático

Solicitar a la computadora que genere un programa (MODELO)
(ya que mi cerebro humano limitado no es capaz de ello)
que sea capaz de predecir un dato en base a un histórico de datos.

## Deep learning

Machine learning con gran cantidad de datos y complejidad en el procesamiento
Se basa en el uso de GPUs

# Inteligencia Artificial

Tratar de que las máquinas simulen ciertos comportamientos / pensamientos de los humanos.
El machine learning es una técnica de IA.


---

# Estadística

Es una ciencia (independiente de las matemáticas) que estudia qué? Poblaciones 

Población: Conjunto de individuos(personas o no) que comparten unas
características, objeto de estudio y análisis

Población: Habitantes de España: 
- Territorio                España!
- Moneda que usan           EURO                            Aburrido: CONSTANTE !
- Festivos nacionales       Todos los mismos
- Lengua                    Español, Catalán, Gallego...    VARIABLE !
- Color de ojos             Marrón, verde, negro, azul      VARIABLE 

Para estudiar esas características en la población, debo medirlas en los individuos.
Para medirlas necesito una ESCALA DE MEDICIÓN:
- Escalas cualitativas
  - Nominales (viene de nombre)
        No es sino un conjunto de nombres arbitrarios que asigno a cada una de las formas en las que puede presentarse la característica.
        Lengua que hablan/escriben/leen: Español, Catalán, Euskera...
        Código postal: 28850 27654 19200 01659

        Al asignar estos valores a los individuos puedo: CLASIFICARLOS
  - Ordinales (orden)
        No es sino un conjunto de nombres que llevan una relación de orden, que asigno a cada una de las formas en las que puede presentarse la característica.
        Me informan del grado / nivel en el que un individuo presenta la característica.

        Nivel de estudios: Primaria < Secundaria < Bachiller < Grado < Master < Doctorado
        Número de portal en el que vives: 17, 29, 118

        Al asignar estos valores a los individuos puedo: CLASIFICARLOS + ORDENARLOS

- Escalas Cuantitativas
    Se caracterizan por CANTIDADES <- UNIDAD DE MEDIDA !
        - Número de hijos que tiene una familia: Ud medida? hij@: 0 hijos, 1 hijo, 2 hijos
        Al asignar estos valores a los individuos puedo: CLASIFICARLOS + ORDENARLOS + OPERACIONES MATEMÁTICAS
    - Intervalo     (El VALOR CERO NO ES UN CERO ABSOLUTO) Puedo sumar y restar y PUNTO
        Disponible en cuenta corriente: -100€ 500€
        Temperatura: 20º -5º 10º
    - Razón         (El VALOR CERO SI ES UN CERO ABSOLUTO) Puedo +, -, *, /
        Número de hijos: 0 hijos, 1 hijo
        Salario: 1000€ 2000€, 17000€

Cambios de escala de medición:
    Cualquier variable en escala Cuantitativa puedo medirla en escala ordinal .
    Y cualquier variable en escala ordinal puedo medirla en escala nominal .
        Número de hijos: 1 hijo... 4 hijos...                       CUANTITATIVA
                         NO, POCOS, ALGUNOS, MUCHOS, DEMASIADOS     ORDINAL
                         NO / SI                                    NOMINAL

## Estadística descriptiva

El conjunto de técnicas que nos ayudan a:
- resumir información 
- Presentar esa información
para hacerla más potable. Que sea capaz de entenderla.

# Técnicas:

# ESTADISTICA DESCRIPTIVA UNIVARIABLE !!!!

## Tabla resumen de los datos: Tabla de frecuencias

Frecuencia? Número veces que ocurre algo. Por si misma es una variable CUANTITATIVA DE RAZÓN.
Número de personas que hablan una lenguaje: FRECUENCIA !

                     Freq. ABSOLUTO     Feq. VALOR RELATIVO     FREQ ACUMULADAS
    Color de ojos:  Personas            % Personas              ABS         REL
        Marron          10                  17%                 10          17%
        Verde           20                  33%                 30          50%
        Azul            15                  25%                 45          75%
        Negro           15                  25%                 60          100%
        ...
   * NOTA: Las frecuencias acumuladas solo tienen sentido si?
            Puedo ordenar los valores de la variable: ESCALA ORDINAL !

   * NOTA 2: Esa tabla también la puedo representar gráficamente: BARRAS / TARTA(SECTORES)

Qué necesito para montar una tabla de frecuencias? PODER CLASIFICAR A LOS INDIVIDUOS.
Qué tipo de escala me permite clasificar a sujetos? Cualquiera
    * Nota: Para las variables cuantitativas que se presentan con muchos valores diferentes, la tabla de frecuencias, nos aporta poco. No resume casi.
      * En este escenario: Clasificar a los individuos en tramos / rangos / intervalos
        Al hacer esto, dejo de usar una escala CUANTITATIVA y paso a una escala ORDINAL !
        0-500€      =       Poco
        500-1000€   =       Algo
        1000-2000€  =       Algo más
        +2000€      =       Algo algo más

En ocasiones queremos resumir aún más la información:
## Estadísticos:

### Estadísticos de tendencia central:      POR DONDE VAN LOS TIROS ! GROSO MODO !

  - Moda        El valor que más veces aparece (el de mayor frecuencia). Lo que está de "moda"
        Qué necesito para calcular una moda: TABLA DE FRECUENCIAS
        Qué escala de medición necesito para calcular una moda: A cualquiera
  - Mediana     El valor que divide a la población en 2 grupos "iguales" del mismo tamaño (más o menos)
        Cómo se calcula:
            Alturas de personas: 150, 170, 180, 175, 190
                Mediana: 1º Ordeno:  150 170 [175] 180 190: Mediana = 175
            Hijos de familias:   0 , 1, 4, 2, 3, 1, 2, 0
                Mediana: Ordeno: 0, 0, 1, 1 [] 2, 2, 3, 4,. Mediana = 1.5
        Qué escala de medición necesito para calcular una mediana: Ordinal o Cuantitativa
  - Media       El resultado de una triste fórmula matemática. 
                Representa la contribución de cada individuo al total.
        Cómo se calcula? Sumado los datos y dividiendo entre el total de sujetos:
        Qué escala de medición necesito para calcular una media: Cuantitativa

    TIPOS DE VARIABLE / ESTADISTICO
                                MODA    MEDIANA MEDIA 
            Nominales            √        X     X
            Ordinal              √        √     X
            Cuantitativas        √        √     √

    La moda en general aporta poco... Por ende: en variables ordinales y cuantitativas, paso de ella.
            Nominales: MODA
            Ordinales: MEDIANA
            Cuantitativas: Mediana / Media ? Cuál? Depende. De qué? 
                    DE LA SIMETRIA DE LA DISTRIBUCION
                        Distribución más o menos simétrica: MEDIA ES MUY REPRESENTATIVA DEL COLECTIVO
                        Distribución muy asimétrica: LA MEDIA ES MUY POCO REPRESENTATIVA DEL COLECTIVO
                Esto se debe a que la media se deja influir mucho por los valores extremos.
                    La media NO ES UN INDICADOR ROBUSTO.
                    La media es un indicador SUFICIENTE (usa todos los valores)
                La mediana no se ve influida por los valores extremos: ES UN INDICADOR ROBUSTO
                    La media es un indicador NO SUFICIENTE (no usa todos los valores)

    # Ejemplo:

        ## Villa-arriba de arriba (10 vecinos)
            5 5 5 10 10 10 10 15 15 15
            Media de contaminación de los vecinos de VAA?   10 g CO/dia
            Mediana:                                        10 g CO/Dia = Media

            ^ frecuencia
            |
            |          X                    X
            |    X     X     X              XX  X
            |    X     X     X .          XXXX|XXXX
            |    X     X     X          XXXXXX|XXXXX
            |----5-----10----15-------------a-H-c------> X: Los valores de la variable
                       ^ Mediana
                         Media
                         Moda
                * La distribución de una variable es la forma del gráfico en el histograma

        ## Villa-arriba de Abajo
            5 5 5 5 [5 5] 5 5 5 1000
            Media: VVAb? 1045/10 =                          104,5 g CO / dia
            Mediana:                                          5 g CO/dia

            ^ frecuencia
            |    X          Distribución asimétrica POSITIVA
            |    X
            |    X
            |    X
            |    X                                                              x
            |----5----100-----200---------------------------------------------1000------------->
                                                                    X: Los valores de la variable
                 ^ Mediana
                            ^ Media
                                     | X
                                     | X
                   x                 | X                  x
                -(-955)--------------0-5----------------1000---->
                                       ^ MEDIANA
                                         MEDIA 
    GRAFICO para representar estos datos? Variables cuantitativas: HISTOGRAMA / BOXPLOT

    Un histograma es como un gráfico de barras. Se parece mucho.

Indique su grado de satisfacción con X? 0-10 -> VARIABLE ORDINAL
                                        poco satisfecho.... muy satisfecho
    Lo mido en 700 sujetos.. y luego enchufo la media: ESTA BIEN ESTO? 
    De media los sujetos están satisfechos un 7.65


    Tipos de mascotas:      TABLA DE FRECUENCIAS
        Perro       100 
        Loro         23
        Gato         98
        Cocodrilo     0

    Esto se representaría en un gráfico de barras:

    ^ Frecuencia
    |
    |   XXX    XX
    |   XXX    XXX
    |   XXX    XXX    XXX
    |----------------------- Valores de la variable
        perro  gato  loro 

# OBJETIVO: RESUMER LA INFORMACION para entenderla mejor

## Calcular los índices de tendencia central: SIRVEN PARA VER POR DONDE VAN LOS TIROS!

## Indices de dispersión:               SIRVEN PARA ESTIMAR CUANDO LOS DATOS CAMBIAN CON RESPECTO A LA TENDENCIA CENTRAL

## VARIANZA ---> RAIZ DE LA VARIANZA = DESVIACION TIPICA: Se basan en el calculo previo de la MEDIA
* NOTA: Cuando tiene sentido usarlos? Solo los usamos si la MEDIA es representativa del colectivo!

Cómo se interpreta: 
Salario medio de 1750€, con una desv. típica de 250€: REGLA DE CHEVICHEV:
Que si abro una desv. tipica alrededor de la media, da igual la forma de la distribucion, siempre encuentro dentro al menos el 50% de la población: LA MAYOR PARTE DE LA POBLACION (la más representativa, pòr estar entorno a la media)
La mayor parte de la gente (al menos el 50%) gana entre 1500€-2000€

Alturas de personas: Portales

Portal 1
    170 170 180 180
    Media:   175 cm
    Mediana: 175 cm
    -5   -5   5   5 ---> Media desviaciones a la media: 0
                    ---> Media los valores absolutos de las diferencias a la media: DESVIACION MEDIA !   5 cm
    25  25  25  25  ---> Media de los cuadrados de las diferencias a la media: 25cm2 = 5cm
Portal 2
    160 175 175 190
    Media:   175 cm
    Mediana: 175 cm
    -15  0 . 0 . 15 ---> Media : 7.5 cm
    225 225 0 0 : 450/4 : 112,5cm2 = 10.5 cm
Portal 3
    165 165 185 185
    Media:   175 cm
    Mediana: 175 cm
    -10 -10  10  10 ---> Media: 10 
    100 x 4 = 400/4 = 100 cm2 = 10cm
Portal 4 
    175 175 175 175
    Media:   175 cm
    Mediana: 175 cm
    0   0   0   0   ---> Media: 0
    0+0+0+0 = 0 -> Dev. tipica: 0cm -> Constante! ABURRIDO !
Portal 5
    165 175 175 185
    Media: 175
    Mediana: 175
    -10  0 . 0 . 10 --> Desviación media: 5
    100 0 0 100 -> 200/4 = 50: Desv. Tipica: 7.1 cm
MORALEJA: NUNCA JAMAS EN LA VIDA puedo poner en un informe un INDICE DE TENDENCIA CENTRAL (el que sea) sin...


### En el caso de usar la MEDIANA como indice de tendencia central, su indice de dispersion asociado es el RANGO INTERCUARTILICO

RIC = Q3-Q1
RSIC = (Q3-Q1)/2: Que tiene la misma interpretación que la DESVIACION TIPICA.

# Medidas de posición

Valor de la variable que deja por debajo una determinada parte de la población.

Mediana:  Divide a la población en 2 partes iguales
Cuartiles: Dividen a la población en 4 partes iguales: Cuántos cuartiles tengo? 
Deciles: 
Percentiles
                
                 Mediana
            Q1     Q2      Q3
    --------|-------|-------|---------
      25% .    25% .   25% .    25%

# ESTADISTICA DESCRIPTIVA MULTIVARIABLE !!!! ---> ESTOES LO GUAY ! Y lo que me permite hacer modelos predictivos: ML, DL, DM

El conjunto de técnicas que me permiten identificar relaciones entre variables: CORRELACIONES

Dependiendo de los tipos de variables (sus escalas de medición), tendré distintas técnicas que podré usar:

## Nominal vs Nominal

    Voy a un pueblo Y A PRIORI conozco que en ese pueblo hay 50% hombres y un 50% de mujeres
                  A PRIORI      ESTIMACION A PRIORI             Ahora voy y entro ... y cuento la realidad
                                    HOMBRES     MUJERES             HOMBRES             MUJERES     Me escaman estos datos?             Cuánto me escaman?
        TREN    (200 personas)        100         100                  95                  105      NO ME ESCAMA !                      POCO
        BUS     (50 personas)          25          25                  30                   20      MAS O MENOS ... pero algo más       ALGO
        TIENDA  (10 personas)           5           5                   4                    6      NO ME ESCAMA                        POQUITO
        MEDICO  ( 80 personas)         40          40                   1                   79      Esto me vuelve loco !!!!            MONTONON
        .....
        LOCAL                                                           55                   0
        TOTAL                                                          185                 185       
        Entre esas variables: En la combinación: SEXO / Ir al médico hay una relación: Ya que los valores esperados no son iguales a los encontrados.
            ^^ HALLAZGO = CORRELACIÓN. GINECOLOGO
        No hay relación entre ir en tren y el sexo. Por qué? porque los valores esperados coinciden bastante con los reales (encontrados)

        El problema es que las relaciones no son SI o NO / Blanco o Negro. 
        La estadística nos da una forma de cuantificar esas correlaciones:
        En este caso concreto: Estadístico: ChiCuadrado: Cuánta relación hay entre 2 variables NOMINALES
        Ese estadístico se calcula contabilizando los cuadrados de las diferencias entre valores esperados y encontrados, racionalizados a los esperados.
        Un problema que tiene chiCuadrado es que su valor está entre 0 e INFINITO.. 
        - Por lo tanto si me da 0 entre 2 variables: Conclusión: No hay relación entre las variables
        - Si me da 27...conclusión? NPI.
        - Lo que hacemos es usar otros estadísticos que se basan en ChiCuadrado:
        - V Crammer, Coef. Contingencia, Coef. Phi: 0...1
              - 0 No hay relación
              - 1 Hay relación máxima
    * Qué pensais, que me interesan cosas que guarden mucha relación entre si o poca? TODO !!!! Y a veces descartaré grandes relaciones en favor de pequeñas relaciones.

## Nominal x Ordinal (Rango salarial, SEXO)
- Calcular el ChiCuadrado y derivados
- Estudio de comparación de medianas: Mediana de Rango salarial para cada sexo

## Nominal x cuantitativa
- Calcular el ChiCuadrado y derivados
- Estudio de comparación de medianas: Mediana de Rango salarial para cada sexo
- Estudio de comparación de medias:   Media   de Rango salarial para cada sexo

## Ordinal x Ordinal
- Calcular el ChiCuadrado y derivados
- R Spearman

## Ordinal x cuantitativa
- Calcular el ChiCuadrado y derivados

## cuantitativa x cuantitativa
- Calcular el ChiCuadrado y derivados
- R Pearson

Modelo predictivo de ML: Lo que hacemos es : Basándome en variables que presentan mucha o poca relación con una variable (la que quiero predecir) buscar la ecuación matemática que me permite hacer la mejor predicción posible.

### Hay relaciones que se dan entre 3 variables... O entre 4 ... o entre 5 variables.




# Ejemplos de correlaciones:

# Ejemplo 1

Población: Personas (humanos) entre 0 y 14 años
Relación entre la edad y la altura. Hay mucha o poca?  MUCHA---> PEDICCIONES BUENAS:
        Si tengo una personita de 0.5 años ... Cuál es su altura?  40-50cm
        Si tengo una personita de 14 años:                         130-150cm

Relación entre altura y peso. Mucha o poca? MUCHA !!!!!
Si os digo que tengo una personita de 5 kilos: Estimación de la altura? 50cm
si os digo que tengo una personita de 65 kilos:                         150cm

Relación entre altura y sexo? MUY POCA RELACION
Os digo que tengo una persona MUJER (entre 0 y 14 años) . Estimación de la altura? NPI 40-160

Si fueseis médicos, que datos usaríais para estimar altura: EDAD, PESO, SEXO? EDAD y PESO... pero en cambio, los médicos que usan? En las tablas de percentiles: EDAD y SEXO

Altura , Edad, Peso, Sexo

Edad x Altura TIENEN MUCHA RELACION
Peso x Altura TIENEN MUCHA RELACION   COLINEALIDAD
Edad x Peso   TIENEN MUCHA RELACION

Altura =F(Edad, Peso)
Lo que me cuenta el peso... básicamente ya me lo ha contado la edad.
Altura = F(1 año, 6 kilos)
Sexo es una variable que no guarda apenas relación con edad
El sexo me cuenta muy poco: Si es niña +3cm. Si es niño -3cm

# Ejemplo 2

Conocimientos de matemáticas y la altura de una persona: NO HAY RELACIÓN 
Si miro los datos entre personitas de 0 a 20 años... ENCONTRARE UN HUEVO DE RELACION
       Mates?                       
50 ->  NPI                              Aquí hay un problema: TENEMOS UNA RELACION ESPURIA: Contaminada por otra variable: EDAD
100 -> sumar y restas
180 -> Saben un huevo de mates

Altura x EDAD
Saber de mates x EDAD

PSICOLOGOS !

Variable: Número de veces que se cae un servidor!           Cuantitativa: Puedo hacer una medición directa del dato.
Variable que es: ALTURA DE UN EDIFICIO: Medida directa
                                        Medida indirecta:  Medir la sombra! Pitagoras al canto!

Variable Grado de ansiedad. No soy capaz ni de definir la variable! Mucho menos de darle una escala ... Ni tengo un aparato para medirlo.
            Ritmo cardiaco
            La cantidad de veces que me despierto por la noche
            Tiempo hasta quedarme dormido
         Nivel de depresión
         Nivel de satisfacción con mi banco!
            Medición: Iluminao: llamas por teléfono y le preguntas! o le mandas un correo!
            El tiempo que llevo contratado
            Si he contratado más productos
            La cantidad de reclamaciones que he abierto

TECNICAS DE REDUCCION DE DIMENSIONES: PCA, Análisis factorial, Análisis de clustering KMEANs