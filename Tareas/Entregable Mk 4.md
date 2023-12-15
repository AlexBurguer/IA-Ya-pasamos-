# Ensayo del Conteo de Islas

## Los Ordenadores y sus capacidades superiores
Los ordenadores son capaces de entender un conjunto de valores binarios y establecer una relación entre ellos, diferenciarlos de conjuntos diferentes y hacer comparaciones entre estos a velocidades me millones de milésimas de segundo. Es del resultado de estas relaciones que le permiten percibir y comprender de la misma manera algunos conceptos que son naturales para nosotros, e incluso aquellos que todavía no se presentan en nuestra realidad, como los espacios en diferentes dimensiones, es fascinante como es que la comprensión de estas medidas escalares parecen resultarle ser naturales, a pesar de que no lo son para el ordenador, es en conceptos como estos que podemos decir que de cierta manera piensan como nosotros, esto ha venido de gran ayuda en general, pues nos ha permitido desarrollar programas y aplicaciones que son capaces de analizar estructuras y resolver, modelar y estudiar problemas relacionados.
El problema que se pretende resolver es algo bastante simple pero que al ser poco natural en el entorno de un ordenador, es un poco mas complejo de hacer de diseño para nosotros, el punto principal es la creación de un programa que permita contar aquellos elementos que están separados de otros, el nombre del problema describe con claridad el problema mismo, se trata de contar aquellos objetos que estén separados, esto es, como su fueran islas.
Esto es algo que resulta completamente natural para nosotros, pues, de acuerdo con la teoría de inteligencias múltiples, una inteligencia en particular nos permite realizar estimaciones en cuanto al espacio y tomando como referencia aquello que vemos, pues, es algo similar, ya que lo que estaremos viendo es una especie de medio, no necesariamente debemos de tratar tan literal al problema por su nombre, esto debido a que es posible que podamos ver islas donde no hay agua y eso se puede representar fácilmente con ejemplos como encontrar rocas entre la tierra, o flores entre la maleza, todo esto tiene relación con la vista y la diferenciación que podemos dar de un medio que no nos interesa y los elementos desperdigados dentro del medio que si nos interesan, en todos los casos podremos ver que nuestra base para saber si se trata de uno u otro es el color que tienen, en el caso de las rocas, estas pueden ser mas oscuras o mas claras que la tierra, esto permite tener un contraste con el medio y diferenciar al elemento que si nos interesa, lo mismo se puede decir que pasa en cualquier ejemplo de islas que encontremos, en el caso de las flores, estas están llenas de colores, mientras que el medio, que sería todo lo que rodea a la flor y no nos interesa, ya puede ser verde o marrón, lo único que debemos de hacer es diferenciarlo bien para poder reconocerlo como un objeto que si sirve o que vamos a ignorar.
Esta capacidad nuestra viene desde el momento en el que el hombre empezó a explorar el mundo, pues, esos momentos eran verdaderamente difíciles y encontrar alimento o diferenciar el peligro de la seguridad es algo que podía hacer la diferencia entre la vida y la muerte, todo esto involucra a nuestros ojos, que son capaces de captar una gran gama del espectro del color, y gracias a este podemos ver la frecuencia de luz que refleja un objeto con la incidencia de la luz, de esta manera es que podemos ver los frutos y diferenciarlos de las plantas, así como todo lo demás en este mundo, el color es tan fundamental para la visión, que sirvió para múltiples elementos de la naturaleza para facilitar su trabajo, como ejemplo podemos ver una gran cantidad de animales que tienen tonalidades de color similar al medio donde son nativos, de allí que los animales del desierto sean marrones o de la selva sean verdes, es cierto que algunos parecen no tener esta cualidad pero es debido a otro tipo de adaptación y de configuración que les da diferentes características, esto por supuesto que representa una ventaja, pues los felinos del desierto pueden prepararse para sorprender al enemigo y tomando en cuenta que los sentidos primitivos de estos animales fueron desarrollados primero que el humano, el hombre tenia que estar siempre atento con la mirada en busca de posibles peligros, fue así como el hombre sobrevivió y se llevo consigo esa habilidad, ahora esta habilidad de ver y distinguir elementos se ha hecho tan natural en nosotros que necesitábamos que nuestra creación también la tuviera, de manera que hemos hecho a las inteligencias artificiales con capacidad de albergar módulos que les permiten tener las mismas características que nosotros, como la capacidad de ver y entender espacios.

## Analisis del problema a resolver
Dentro de lo que es la resolución del problema, se nos pide que se genere un método iterativo y otro recursivo, el primero de ellos refiere a la utilización de alguna clase de ciclos con la finalidad de que tenga una repetición constante, además, la recursividad permite tener cierta intuitivita, ya que con el proceso general puede ayudar a entender un problema completo.
Esto se ha hablado ya en las clases de inteligencia artificial y el argumento principal es que como datos de entrada debíamos de tener una clase de mapa, que en este caso se representa con una matriz n, m, que tiene algunos segmentos ya sea con un dato o con un color en concreto, realmente, su contenido no es relevante siempre que sea diferente a los casos que requiera, es decir, no importa si los datos vacíos se representan con un cero y los llenos con un uno, o con un color blanco los vacíos y un color negro los llenos, siempre que los datos sean diferentes el programa de ordenador será capaz de entender que uno pertenece a un conjunto distinto del otro.
Si bien podemos realizar un programa que pueda recorrer la matriz y cuente los unos que hay en esta matriz, no podemos saber con certeza que estos unos están separados unos de otros para ser considerados islas, por lo que debemos de contar con mas validaciones que hagan posible saber si están pegados entre si y una vez que se contabilizan quitarlos de la matriz.
La solución del problema esta dada por los problemas del sencillo programa del párrafo anterior, pues se necesita la iteración para recorrer la matriz y se necesita la recursividad para saber si los puntos están conectados, contarlos e ignorarlos una vez que pasen por el conteo.
Para nosotros es bastante fácil reconocer las islas, pero debemos de tomar en cuenta que la lectura de una matriz no es como mirarla, para que el programa sepa qué hay en un espacio, primero tiene que leerlo, y cuando esto suceda, no podrá ver que habrá en el vecino próximo hasta que pase por él, es por esto que es tan difícil realizar este tipo de aproximaciones.
Esto por supuesto, no representa un problema cuando se trata de inteligencia artificial, aun estamos hablando de programas simples de computadora que realmente no piensan, tampoco es que sea tan diferente, pero es mucho más fácil cuando tienes sistemas de reconocimiento como si lo haría una inteligencia artificial.

## Solución
De acuerdo con lo que una eminencia en el campo de la inteligencia artificial estipuló:
El programa recorrerá la matriz de manera iterativa, cada vez que se encuentre con un trozo que si contenga datos, este de manera recursiva mirará a los cuatro cuadrantes que se encuentran alrededor de este cuadrante que si contiene datos en busca que dé más cuadrantes con datos y solo hasta que se haya asegurado de que no hay datos alrededor podrá contabilizar este dato o conjunto de datos de ser una isla, acto seguido se procederá a borrar todo ese conjunto de datos, y seguirá recorriendo la matriz desde el punto en que lo dejo, la razón por la cual se debe de borrar, es debido a que puede entrar en confusión si la isla abarca parte de las casillas por las que todavía no se ha iterado si esto pasa y no se borra la isla, el algoritmo volverá a recorrer esta isla y la volverá a contabilizar, esto provocara que nos de un resultado erróneo, pero hay una solución para esto, podemos crear una copia de la matriz y trabajar con esta, de modo que la matriz original seguirá teniendo la misma cantidad de islas que con las que entró y de cualquier forma nos daría un resultado preciso.
Este problema en particular me pareció muy interesante, hace algunos documentos hablábamos de como programas sencillos eran usados para resolver problemas gordos, pues este es uno de esos casos, dentro de la medicina se utiliza este problema para estudiar las células y detectar posibles anomalías.