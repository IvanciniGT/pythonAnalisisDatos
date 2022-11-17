# Datos de los coches:

## Objetivos

1- Entender los datos, y como se relacionan entre si

2- Con respecto a que me vaya a dar un parte:                                   MODELO DE MACHINE LEARNING
    A- Intentar adivinar si va a dar el parte o no                              MODELO DE CLASIFICACION
        SALIDA DE ESE POTENCIAL MODELO:      0  |  1
    B- Intentar estimar la probabilidad de que me de vaya a dar un parte!       MODELO DE REGRESION
        SALIDA DE ESE POTENCIAL MODELO SERÁ: 0.....1
        Porque vaya a usar ese dato para cobrarle más o menos pasta, proporcionalmente a esa probabilidad(riesgo)

MODELO A:

Para decidir si a una persona le pongo un 0 o un 1... lo haré en base a una probabilidad P
    P< Limite = 0     Limite = 50%
    P> Limite = 1
    
    | Probabilidad
 1  |                        ...........     TARIFA C        Quiero un modelo con un gran poder de clasificación
    |                       .
    |                       .     
    |              .........                 TARIFA B        Quiero un modelo con un gran poder de clasificación
    |             .
    |            .
 0  | ...........                            TARIFA A
    |----------------------------------------- modelo(a,b,c,d)

    Coste del seguro de coche: Tener a mis sujetos clasificados por niveles de riesgo (probabilidad de darme un parte)

MODELO A:
    
    | Probabilidad o una variable la que sea: COSTE
 b  |                   ..........                     Quiero un modelo con un gran poder de clasificación
    |            ...... 
    |       .....                       Una tarifa proporcional al riesgo
 a  | ......
    |------------------------------- modelo(a,b,c,d)

    Costes del seguro médico

    
Darme vuestra mejor estimación posible, a la vista de los datos que tenemos para saber si unna persona NUEVA va a dar un parte:
    p(dar parte)    = 31%
    p(no dar parte) = 69%

MODELO 1: PREDICCION: NO VA A DAR PARTE
    
Este es un modelo ya... Este es del que parto !
                    ESTIMACION
                    NO          SI
    REALIDAD
        NO         6967         0       6867
        SI         3133*        0=A     3133
                   10000        0
    
    DATO * = FALSOS NEGATIVOS! = 30%
    DATO ** = FALSOS POSITIVOS! = 0%
    En cuantos acierto al hacer la predicción? 
        Al decir que no:  70% *****
        Al decir que si:   0% ***** 
        Qué me interesa?
        - me interesa más acertar en los SIs o en los NOs? 
            - Los SI
            - Los NO
            - AMBOS ! El problema es que esto es IMPOSIBLE !
            O maximizo uno, o el otro, los 2 a la vez no puedo!

MODELO 2: PREDICCION: SI VA A DAR PARTE
    
                    ESTIMACION
                    NO          SI
    REALIDAD
        NO         0             6967**       6867
        SI         0*            3133         3133
                   0            10000
    
    DATO *  = FALSOS NEGATIVOS! = 0
    DATO ** = FALSOS POSITIVOS! = 70%
    
    En cuantos acierto al hacer la predicción? 
        Al decir que no:   0% *****
        Al decir que si:   30% ***** 
        Si lo que me interesa es saber si dan parte!  DATO A
                   

A veces me interesa acertar mucho. En los SIs o en los NOS
A veces me importa una mierda acertar en los SIs o en los NOs. Lo que interesa es minimizar los Falsos POSITIVOS O NEGATIVOS

# EJEMPLO: Imaginad que hago un test de deteccion de ????


                       PRUEBA A
                    NO          SI
    REALIDAD
        NO          35          5        40
        SI          10          50       60
                    45          55      100
    
    Tasa de éxito de mi prueba A ?
        Qué es el éxito?                    %
            Acertar en los SIs?              50/60   = 83%
            Acertar en los NOs?              35/40   = 87,5%
            Minimizar los Falsos positivos?   5/40   = 12,5%
            Minimizar los falsos negativos?  10/60   = 17%
            Efectividad de la detección      50/55   = 90,1%
            
            Si la prueba es de detección de covid:
            
            Minimizar los falsos negativos!
                Lo que me interesa es que no haya gente por la calle que si tenga covid !!!! 10 <<<<
                    Y eso hará que haya más gente que no teniendo covid diga yo que si lo tienen 
                            -> Gente sana se queda en su casa 15 días  (vaya putadita !)
    
            Si la prueba es de detección de cancer:
                Minimizar los falsos positivos!
                Primo el no decir que una persona sana tiene cancer.. eso implicaría que le voy a hacer quimio...
                Y ESO ES MUY JODIDO !
                Eso irá en contra de dejar a gente que si tiene cancer, sin detectar. 
                            -> Ya les haré otra prueba !



    | Probabilidad
 1  |                        ...........     DETECTADO
    |                     ...    
    |                  ...              ^
    __________________________________________          
    |               ..                  v
    |             ..
    |            .
 0  | ...........                            NO DETECTADO (covid, cancer, ostion con el coche, no paga la hipoteca)
    |----------------------------------------- modelo(a,b,c,d)


DECITION TREE       1 modelo

RANDOM FOREST       genera un huevo de DECITION TREE



    | Probabilidad
 1  |            ....................     DETECTADO
    |            .    
    |            .             ^
    __________________________________________          
    |            .                  v
    |            .
    |            .
 0  | ...........                            NO DETECTADO (covid, cancer, ostion con el coche, no paga la hipoteca)
    |----------------------------------------- modelo(a,b,c,d)


                                                                                Dar un parte
AGE                             Más mayor más responsable                       DISMINUIR
                                Más mayor más experiencia                       DISMINUIR
                                Más mayor menos habilidades                     AUMENTAR
GENDER
                                Mujer más prudente                              DISMINUYE
                                Mujer suele tener más cosas en la cabeza        ?
RACE
                                En serio ? Asi estamos ?
DRIVING_EXPERIENCE      
    Antigüedad del carnet       A priori: A más años más experiencia            DISMINUYE
EDUCATION
                                A priori no... Podriasmos rascar un poco
INCOME
    pasta que gano!             A más income mejor vehiculo... 
                                        mejor vehiculo tiene mejores sistemas de seguridad  DISMINUYE
CREDIT_SCORE
                                A más credit score mejor vehículo
VEHICLE_OWNERSHIP               Si soy propietario más responsable              ********
                                                    o menos 
VEHICLE_YEAR
                                A más antigüedad  peores sistemas de seguridad  AUMENTA
MARRIED
                                Si estoy casado: Más probabilidad de multiuso   AUMENTAR
                                Si estoy casado, puedo comportarme un poco más responsablemente
CHILDREN
                                Si tengo hijos puedo comportarme un poco más responsablemente
                                Pero me van a volver loco cuando llevo atrás
                                Si los hijos usan el coche....
POSTAL_CODE
                                Sitios con mayor probabilidad de accidente
                                También guarda relación con la pasta
                                Característcias del vehículo
                                Infraestructura
ANNUAL_MILEAGE
                                A más: Más probabilidades de accidente: NIVEL DE EXPOSICION AL PELIGRO 
                                A más, más experiencia                : EXPERIENCIA 
VEHICLE_TYPE
                                A priori deportivo puede incrementar riesgo
                                
SPEEDING_VIOLATIONS             Si aumentan, más probabilidad
DUIS
                                EXPOSICION AL PELIGRO MAYOR
                                RESPONSABILIDAD 

PAST_ACCIDENTS                  0 Si es nuevo... habrá que ver 
                                0 llevar 20 años... cuidao !
                                Esta varioable habla de todo !!!
