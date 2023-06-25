# TPF_1-Cecilia.Miranda-Ezequiel.Zelaya-
En esta documentación, nos complace presentarles el juego "Hoppity" y las funciones implementadas para su desarrollo. "Hoppity" es un emocionante juego de estrategia en el que el objetivo es llevar todas las fichas de uno al lado contrario del tablero. Este juego ha sido creado por Cecilia Miranda Tito y Gustavo Ezequiel Zelaya González en el primer semestre del 2023.

En esta documentación, encontrarán una descripción de las reglas del juego, así como una explicación detallada de las funciones implementadas para su funcionamiento. Estas funciones han sido diseñadas con el fin de brindar una experiencia fluida y emocionante a los jugadores.

A continuación, se presenta un resumen de las funciones implementadas:

void tablerosPuntaje: Esta función genera dos tableros diferentes dependiendo de los escenarios posibles en el juego. Estos tableros permiten determinar la ruta más ventajosa para la computadora, considerando el camino más ventajoso y evaluando la ventaja que lleva el contrincante dependiendo del lado que se escoja.

void cleanBuffer: Esta función se encarga de limpiar el buffer, asegurando que no queden datos residuales que puedan afectar el funcionamiento del juego.

void tableroInicial: Esta función posiciona las fichas en el tablero en sus posiciones iniciales, preparando el escenario para el inicio del juego.

void imprimirTablero: Utilizamos esta función para verificar la impresión del tablero en la terminal, asegurando que se muestre correctamente durante el transcurso del juego.

typedef struct string: Esta estructura de datos permite al usuario cargar la configuración de la partida, eligiendo la pieza y el turno. Se utilizan bucles con while para asegurar que solo se ingresen los valores requeridos, y se devuelven los mismos mediante punteros.

typedef struct coord: Esta estructura de datos se utiliza para almacenar las coordenadas de una ficha en el tablero, representando su posición en las coordenadas x e y.

int isJumpable: Esta función recibe el tablero actual, la ficha seleccionada y la posición a la que se desea mover, y determina si la ficha seleccionada y el destino son aptos para realizar un movimiento de salto en el tablero.

int checkadyacente: Esta función recibe el tablero actual, la ficha seleccionada y la posición a la que se desea mover, y determina si la ficha seleccionada y el destino son aptos para realizar un movimiento adyacente en el tablero.

typedef struct siguiente: Se crea un tipo de dato que contiene las coordenadas de la ficha que se está analizando, y se inicializa un tablero falso que se utilizará para generar casos hipotéticos de jugadas.

typedef struct jugada: Esta estructura de datos contiene las coordenadas de la ficha que se está analizando, la ruta de movimiento planificada, el puntaje que generaría el movimiento en el tablero hipotético y un contador de las posibles jugadas que se pueden realizar.

void generarAdyacentes: Esta función genera todas las posibilidades de movimiento adyacente para todas las fichas de la computadora, guardando la mejor ruta que puede generar cada ficha en el tablero de puntajes, según su posición en el tablero.

void generarSaltos: Esta función genera todos los posibles saltos que se pueden realizar con todas las fichas del jugador, considerando el mejor camino que puede tomar cada ficha según su posición en el tablero de puntajes.

int predit_salto: Esta función intenta predecir futuros saltos, ya que los saltos son las jugadas más ventajosas en este juego. Busca posibles saltos y guarda las mejores coordenadas para el movimiento.

void generarTablerosPrueba: Esta función genera tableros de prueba dependiendo de la cantidad de rutas de movimientos encontradas, y coloca los mejores movimientos posibles para cada ficha con posibilidad de movimiento.

void generarPuntajes: Esta función recorre todos los tableros de prueba uno por uno, buscando todas las piezas y evaluando el puntaje que ocupan en el tablero de puntajes, dependiendo del lado de inicio. Las fichas de la computadora suman puntos, mientras que las fichas enemigas restan puntos. Los posibles saltos suman puntos, mientras que los saltos del enemigo restan. Lo mismo se aplica a las fichas adyacentes, pero con un puntaje menor.

Con estas funciones implementadas, el juego "Hoppity" ofrece una experiencia desafiante y entretenida para los jugadores. Esperamos que disfruten de esta documentación y aprovechen al máximo el juego.

Cecilia Miranda Tito
Gustavo Ezequiel Zelaya González
