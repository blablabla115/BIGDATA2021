para mostrar los resultados del apriori se usan 2 data set mas ligeros:
- data 1 : spotify.npy (no se usa y esta comentado)
- dataTest : ejemplo sacado de internet (esta comentado)
- newdataTest : ejemplo con el que se trabajo en clases para probar la libreria apriori (SE USA PARA EJEMPLO)

el modulo get_frequent_itemsets recibe como primer parametro la lista de itemsetS (dataset) en forma de Diccionario por lo que 
el dataset que se uso en clases se modifico a un diccionario

dataset de prueba
newdataTest = {0:['MILK','BREAD','BISCUIT'],
              1:['BREAD','MILK','BISCUIT','CORNFLAKES'],
              2:['BREAD','TEA','BOURNVITA'],
              3:['JAM','JUICE','BREAD','MILK'],
              4:['JUICE','TEA','BISCUIT'],
              5:['BREAD','TEA','BOURNVITA','COOKIES'],
              6:['JUICE','TEA','CORNFLAKES'],
              7:['JUICE','BREAD','TEA','BISCUIT'],
              8:['JAM','JUICE','BREAD','TEA'],
              9:['BREAD','MILK'],
              10:['COFFEE','COOKIES','BISCUIT','CORNFLAKES'],
              11:['COFFEE','COOKIES','BISCUIT','CORNFLAKES'],
              12:['COFFEE','SPLENDA','BOURNVITA'],
              13:['BREAD','COFFEE','COOKIES'],
              14:['BREAD','SUGAR','BISCUIT'],
              15:['COFFEE','STEVIA','CORNFLAKES'],
              16:['BREAD','SUGAR','BOURNVITA'],
              17:['BREAD','COFFEE','SPLENDA'],
              18:['BREAD','COFFEE','STEVIA'],
              19:['TEA','MILK','COFFEE','CORNFLAKES']}
              
############################################################ itemsets frecuentes min_support = 0.1 ########################################################
1 ['BISCUIT']
soporte  0.35


2 ['BOURNVITA']
soporte  0.2


3 ['BREAD']
soporte  0.65


4 ['COFFEE']
soporte  0.4


5 ['COOKIES']
soporte  0.2


6 ['CORNFLAKES']
soporte  0.3


7 ['JAM']
soporte  0.1


8 ['JUICE']
soporte  0.25


9 ['MILK']
soporte  0.25


10 ['SPLENDA']
soporte  0.1


11 ['STEVIA']
soporte  0.1


12 ['SUGAR']
soporte  0.1


13 ['TEA']
soporte  0.35


14 ['BISCUIT', 'BREAD']
soporte  0.2


15 ['BISCUIT', 'COFFEE']
soporte  0.1


16 ['BISCUIT', 'COOKIES']
soporte  0.1


17 ['BISCUIT', 'CORNFLAKES']
soporte  0.15


18 ['BISCUIT', 'JUICE']
soporte  0.1


19 ['BISCUIT', 'MILK']
soporte  0.1


20 ['BISCUIT', 'TEA']
soporte  0.1


21 ['BOURNVITA', 'BREAD']
soporte  0.15


22 ['BOURNVITA', 'TEA']
soporte  0.1


23 ['BREAD', 'COFFEE']
soporte  0.15


24 ['BREAD', 'COOKIES']
soporte  0.1


25 ['BREAD', 'JAM']
soporte  0.1


26 ['BREAD', 'JUICE']
soporte  0.15


27 ['BREAD', 'MILK']
soporte  0.2


28 ['BREAD', 'SUGAR']
soporte  0.1


29 ['BREAD', 'TEA']
soporte  0.2


30 ['COFFEE', 'COOKIES']
soporte  0.15


31 ['COFFEE', 'CORNFLAKES']
soporte  0.2


32 ['COFFEE', 'SPLENDA']
soporte  0.1


33 ['COFFEE', 'STEVIA']
soporte  0.1


34 ['COOKIES', 'CORNFLAKES']
soporte  0.1


35 ['CORNFLAKES', 'MILK']
soporte  0.1


36 ['CORNFLAKES', 'TEA']
soporte  0.1


37 ['JAM', 'JUICE']
soporte  0.1


38 ['JUICE', 'TEA']
soporte  0.2


39 ['BISCUIT', 'BREAD', 'MILK']
soporte  0.1


40 ['BISCUIT', 'COFFEE', 'COOKIES']
soporte  0.1


41 ['BISCUIT', 'COFFEE', 'CORNFLAKES']
soporte  0.1


42 ['BISCUIT', 'COOKIES', 'CORNFLAKES']
soporte  0.1


43 ['BISCUIT', 'JUICE', 'TEA']
soporte  0.1


44 ['BOURNVITA', 'BREAD', 'TEA']
soporte  0.1


45 ['BREAD', 'JAM', 'JUICE']
soporte  0.1


46 ['BREAD', 'JUICE', 'TEA']
soporte  0.1


47 ['COFFEE', 'COOKIES', 'CORNFLAKES']
soporte  0.1


48 ['BISCUIT', 'COFFEE', 'COOKIES', 'CORNFLAKES']
soporte  0.1

#########################################################################  REGLAS GENERADAS ######################################################
CONFIDENCE = 0.5
LIFT = 1.5

1 [['BISCUIT'], ['BREAD']]
lift:  0.8791208791208792
confidence  0.5714285714285715


2 [['COOKIES'], ['BISCUIT']]
lift:  1.4285714285714286
confidence  0.5


3 [['CORNFLAKES'], ['BISCUIT']]
lift:  1.4285714285714286
confidence  0.5


4 [['BOURNVITA'], ['BREAD']]
lift:  1.1538461538461537
confidence  0.7499999999999999


5 [['BOURNVITA'], ['TEA']]
lift:  1.4285714285714286
confidence  0.5


6 [['COOKIES'], ['BREAD']]
lift:  0.7692307692307692
confidence  0.5


7 [['JAM'], ['BREAD']]
lift:  1.5384615384615383
confidence  1.0


8 [['JUICE'], ['BREAD']]
lift:  0.923076923076923
confidence  0.6


9 [['MILK'], ['BREAD']]
lift:  1.2307692307692308
confidence  0.8


10 [['SUGAR'], ['BREAD']]
lift:  1.5384615384615383
confidence  1.0


11 [['TEA'], ['BREAD']]
lift:  0.8791208791208792
confidence  0.5714285714285715


12 [['COOKIES'], ['COFFEE']]
lift:  1.8749999999999996
confidence  0.7499999999999999


13 [['COFFEE'], ['CORNFLAKES']]
lift:  1.6666666666666667
confidence  0.5


14 [['CORNFLAKES'], ['COFFEE']]
lift:  1.6666666666666667
confidence  0.6666666666666667


15 [['SPLENDA'], ['COFFEE']]
lift:  2.5
confidence  1.0


16 [['STEVIA'], ['COFFEE']]
lift:  2.5
confidence  1.0


17 [['COOKIES'], ['CORNFLAKES']]
lift:  1.6666666666666667
confidence  0.5


18 [['JAM'], ['JUICE']]
lift:  4.0
confidence  1.0


19 [['JUICE'], ['TEA']]
lift:  2.285714285714286
confidence  0.8


20 [['TEA'], ['JUICE']]
lift:  2.285714285714286
confidence  0.5714285714285715


21 [['COOKIES'], ['BISCUIT', 'COFFEE']]
lift:  5.0
confidence  0.5


22 [['COOKIES'], ['BISCUIT', 'CORNFLAKES']]
lift:  3.3333333333333335
confidence  0.5


23 [['BOURNVITA'], ['BREAD', 'TEA']]
lift:  2.5
confidence  0.5


24 [['JAM'], ['BREAD', 'JUICE']]
lift:  6.666666666666667
confidence  1.0


25 [['COOKIES'], ['COFFEE', 'CORNFLAKES']]
lift:  2.5
confidence  0.5


26 [['COOKIES'], ['BISCUIT', 'COFFEE', 'CORNFLAKES']]
lift:  5.0
confidence  0.5


