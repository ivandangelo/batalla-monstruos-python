# *tp1-EDD-Python*
--------

## Nombres de los integrantes del Grupo: 

* Fernandez Lucas
* Ledesma Javier
* Ivan Manuel D'angelo

## Decisiones de disenio:

* Elegimos usar un menu por consola de jupyter debido a su sencilles y que no presentaba problemas a la hora de correr el juego.
* Para representar los elementos que un monstruo puede tener se uso una clase Tipologia de tipo enum, donde cada elemento de la clase
tiene dos atributos, el primero el elemento contra el que es fuerte y el segundo contra el que es debil.
* Decidimos usar pickle porque era sencillo y no presentó problemas a la hora de guardar una partida, a diferencia de JSON que no 
acepta todos los objetos nativos de Python.
* Aprovechando el tipado dinámico de Python, varios de los atributos en la clase Monstruo son referenciados directamente desde el 
MenuCrearMonstruo en vez de pasarlos como parametro en la clase Monstruo.

## Descripcion de cada archivo:

__Menues__
* MenuAtaques-- Menú donde se realizan los ataques.
* MenuCrearJuego-- Menú donde se crea el juego.
* MenuCrearMonstruo-- Menú para crear el monstruo.
* MenuInicial-- Se muestran las opciones del menú inicial.
* MenuPersistencia-- Menú donde se permite cargar y guardar la partida.

__Persistencia__
* PersistenciaPickle-- Guarda y carga una partida.

__Tipologia__
* Tipologia-- Almacena los 4 tipos de elementos cada uno con su respectivo elemento fuerte y debil.

__Juego__
* Juego-- Maneja la lógica de crear los personajes iniciar el juego, determinar si terminó el juego y nombrar al ganador.
* Monstruo-- Monstruo con sus elementos y un personaje asociado.
* Personaje-- Personaje con su nombre asociado.

__Raiz__
* JuegoMonstruos-- Launcher para ejecutar el juego
* TestJuego-- Tests de la clase Juego
* TestMonstruo-- Tests de la clase Monstruo
* TestPersonaje-- Tests de la clase Personaje
* TestTipologia-- Tests de la clase Tipologia

##Conclusiones:
Como ya teniamos el proyecto en Java y no hacía falta pensar la lógica, nos facilitó familiarizarnos con la sintaxis de Python y con las ventajas que ésta trae con respecto a Java, como por ejemplo, los with open. Otra clara ventaja es la posibilidad de acceder a los atributos de una clase desde afuera de la misma, ya que nos ayudó a comprimir el código y no hace falta realizar getters ni setters. En cuanto a la persistencia, pudimos agregarle nueva funcionalidad al juego sin requerir de mucho esfuerzo gracias a la facilidad de poder importar nativamente pickle en Python y su simple sintaxis.
