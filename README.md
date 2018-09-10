# TALLER 1 DCA

## Clase Main

Es la clase donde se ejecutan las acciones del aplicativo.

** Atributos:**
- **log:** un objeto tipo Logica que permite llamar los metodos de esa clase.

**M�todos:** 
+ **settings:** Se define el size del cambas que se va a usar.
+ **setup:** se inicializan los elementos una sola vez, por ejemplo, log.
+ **draw:** aqu� se pintan los objetos que vamos a utilizar de las otras clases llamando log.pintar();
+ **mousePressed:** usara el metodo clic de la clase Logica para las acciones press
+ **mouseDragged:** Permite arrastrar los elementos.

## Clase Logica

**Atributos:**
- **app:** Un dato tipo PApplet que nos permitir� usar la librer�a de processing.
- **texto:** Dato tipo string en que el se contiene el archivo de texto.

**M�todos:**
+ **pintar:** este metodo dibuja en el lienzo las figuras que se van a crear a partir de la clase Figura
+ **clic:** ejecuta las acciones de clic para crear o hacer girar objetos.
+ **sacudir:** metodo para hacer caer los triangulos que componen al sol.
+ **arrastrar:** metodo para desplazar el sol de lugar por medio de clic sostenido.

## Clase Figura(Padre)

Es la clase padre que contiene los atributos y metodos que ser�n heredados a los hijos.

**Atributos:**
**app:** Un dato tipo PApplet que nos permitir� usar la librer�a de processing.
**x:** tipo de dato float que representa la posicion en x.
**y:** tipo de dato float que representa la posicion en y.
**tam:** tipo de dato entero que representa el tama�o de la figura.
**char:** tipo de dato caracter que nos permitir� su posterior modificaci�n en el archivo de texto.

**M�todos:**
+ **Figura(int,int)** Constructor de la clase Figura.
+ **pintar:** m�todo para heredar a todos los hijos la acci�n de pintarse.

## Clase Circulo(hereda de padre)

Es la clase donde se va a crear el objeto Circulo.

**M�todos:**
+ **mover:** este m�todo le permite al circulo desplazarse en x a la derecha.
+ **cambiarColor:** este m�todo al oprimir una tecla(c) cambia el color del circulo a amarillo.


## Clase Triangulo(hereda de padre)

Es la clase donde se va a crear el objeto Triangulo.

**M�todos:**
+ **girar:** hace girar a los triangulos que se crean alrededor del circulo, formando un sol.
+ **cambiarColor:** cambia el color de los triangulos a amarillo.

## Clase Rectangulo(hereda de padre)

Es la clase donde se va a crear el objeto Rectangulo.

**M�todos:**
+ **pintar:** pinta el rectangulo.

## Clase Hexagono(hereda de padre)

Es la clase donde se va a crear el objeto Hexagono.

**M�todos:**
+ **pintar:** pinta el hexagono.