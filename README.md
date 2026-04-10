# Solemne 1: Recrear una obra en p5.js Web-Editor
## Indicaciones de la solemne
* Deben recrear con exactitud el dibujo que hicieron en papel milimetrado en un Sketch de P5.js. de 500 X 500 PIXELES.
* Referente elegido: Kazimir Malévich (1879-1935)

## Proyecto
El proyecto consiste en la reinterpretación de una composición geométrica inspirada en el trabajo de Kazimir Malevich, particularmente en los principios del suprematismo, donde la forma pura, el color y la disposición en el espacio adquieren un rol protagónico. A partir de esta referencia, se desarrolló una propuesta visual basada en figuras geométricas simples como triángulos, óvalos, rectángulos y líneas, organizadas en una composición dinámica que busca generar tensión y equilibrio a la vez. El uso de colores planos y contrastantes refuerza esta intención, evocando una estética abstracta que se aleja de la representación figurativa y se centra en lo esencial de la forma.

## Proceso de réplica
El proceso de réplica se realizó mediante la traducción de una imagen a un sistema digital utilizando p5.js, lo que implicó descomponer la composición en sus elementos básicos y reconstruirlos a partir de coordenadas precisas dentro de un lienzo de 500x500 píxeles. Para lograr mayor exactitud, se trabajó sobre una grilla modular que permitió ubicar cada figura en posiciones proporcionales, facilitando la correspondencia entre la imagen original y su versión digital. Este proceso exigió una observación detallada de las relaciones espaciales, proporciones y jerarquías visuales presentes en la obra.

## Dificultades
Una de las principales dificultades del proyecto fue la recreación de los arcos presentes en la composición. A diferencia de las figuras geométricas rectas, los arcos implican trabajar con ángulos, radios y centros que no siempre coinciden de manera evidente dentro de la grilla. Esto requirió múltiples ajustes y pruebas en p5.js, modificando parámetros como el tamaño, la posición y el rango angular de las funciones de arco para aproximarse con precisión al trazo original. Además, el grosor del trazo y su interacción con otras figuras complejizó aún más su representación, ya que pequeños cambios generaban diferencias visuales significativas.

## Conclusión
En conclusión, el proyecto no solo implicó la reproducción de una composición abstracta, sino también la comprensión de un lenguaje visual específico y su traducción a un entorno digital. La influencia de Kazimir Malevich se evidencia en la simplificación formal y en la búsqueda de una composición equilibrada a partir de elementos mínimos, mientras que el uso de herramientas digitales permitió explorar nuevas formas de construir y analizar la geometría en el espacio.

# Dibujo original inspirado en Kazimir Malévich
![IMG_2634](https://github.com/user-attachments/assets/bebe9d6c-d4d3-4b95-bdd3-7821beeecc4c)

# Work in progress
![IMG_2709](https://github.com/user-attachments/assets/71332f7e-a6a3-4be2-a49f-64436c7c3f2c)

# Resultado en p5.js Web Editor
<img width="1000" height="1000" alt="image" src="https://github.com/user-attachments/assets/6184dc17-4b7e-47f1-b262-2d17eb2f9910" />

# Codigo comentado
setup() {
  createCanvas(500, 500);
  background(255, 255, 255
);
  angleMode(DEGREES);
}

function draw() {
  stroke(0); //color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(255, 121, 10); //color del relleno de la figura
  rect(20, 20, 70, 35); //tamaño y coordenadas del rectangulo
  
  stroke(0);//color del contorno
  strokeWeight(30);//tamaño del grosor del contorno
  strokeCap(SQUARE); ////sirve para que el borde sean cuadrados
  fill(255, 255, 255);//color del relleno de la figura
  arc(260 ,-50, 300,300,360, 180);//tamaño y coordenadas de los arcos
  
  stroke(0);//color del contorno
  strokeWeight(3);//tamaño del grosor del contorno
  strokeCap(SQUARE); ////sirve para que el borde sean cuadrados
  fill(255, 251, 10);//color del relleno de la figura
  arc(220 ,10, 120,90 ,360, 180);//tamaño y coordenadas de los arcos
  
  fill(235, 2, 2);//color del relleno de la figura
  triangle(20,70, 250,350, 20, 350 );//tamaño y coordenadas del triangulo
  
  
  strokeWeight(3);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(110, 50, 160, 100);//tamaño y coordenadas de la línea
  
  point(165,105);//coordenadas de un punto
  
   point(170,110);//coordenadas de un punto
  
  point(175,115);//coordenadas de un punto
  
  point(360, 10);//coordenadas de un punto
  
  point(356, 20);//coordenadas de un punto
  
  point(350, 30);//coordenadas de un punto
  
  strokeWeight(20);//tamaño del grosor del contorno
  stroke(5, 34, 171);//color del contorno
  line(330,210, 219, 310);//tamaño y coordenadas de la línea
  
  
   strokeWeight(3);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(342, 38, 310, 70);//tamaño y coordenadas de la línea
  
 stroke(255, 251, 10);//color del contorno
  strokeWeight(20);//tamaño del grosor del contorno
  fill(255, 255, 255);//color del relleno de la figura
  arc(77 ,133, 160,100,230,-340);//tamaño y coordenadas de los arcos
  

  strokeWeight(20);//tamaño del grosor del contorno
  stroke(255, 121, 10);//color del contorno
  line(210,114, 440, 300);//tamaño y coordenadas de la línea
  
strokeWeight(20);//tamaño del grosor del contorno
  stroke(5, 34, 171); //color del contorno
  line(320,6, 13, 300);//tamaño y coordenadas de la línea
  
  stroke(0); //color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(235, 2, 2); //color del rectangulo
  rect(425, 110, 60, 110); //tamaño y coordenadas del rectangulo
  
  fill(255, 251, 10);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(450, 60,90, 40);//tamaño y coordenadas de la elipse
  
  fill(5, 34, 171);//color del relleno de la figura
  stroke(0);//color del contorno
  triangle(400,90, 400,170, 350, 125 );//tamaño y coordenadas del triangulo
  
   point(484,238);//coordenadas de un punto
  point(484,252);//coordenadas de un punto
  
  stroke(0);//color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(255, 251, 10); //color del rectangulo
  rect(474, 270, 16, 70); //tamaño y coordenadas del rectangulo
  
   strokeWeight(5);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(458, 320, 458, 230);//tamaño y coordenadas de la línea
  
  point(458,335);//coordenadas de un punto
  
  strokeWeight(5);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(482, 400, 482, 350);//tamaño y coordenadas de la línea
  
  point(482,415);//coordenadas de un punto
  point(482,430);//coordenadas de un punto
  
  strokeWeight(5);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(482, 446, 482, 490);//tamaño y coordenadas de la línea
  
  
  fill(255, 121, 10);//color del relleno de la figura
  stroke(0);//color del contorno
  triangle(460,350, 460,480, 300, 480 );//tamaño y coordenadas del triangulo
  
    fill(0);//color del relleno de la figura
  stroke(0);//color del contorno
  triangle(300,120, 300,150, 272, 126 );//tamaño y coordenadas del triangulo
  
  fill(255, 251, 10);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(200, 200,100, 50);//tamaño y coordenadas de la elipse
  
  point(250,225);//coordenadas de un punto
   point(240,235);//coordenadas de un punto
  point(230,245);//coordenadas de un punto
  
   fill(0);//color del relleno de la figura
  stroke(0);//color del contorno
  triangle(178,245, 200,275, 220, 247 );//tamaño y coordenadas del triangulo
  
  stroke(0);//color del contorno
  strokeWeight(5);//tamaño del grosor del contorno
  fill(255);//color del relleno de la figura
  arc(100 ,90, 96,80 ,-330, 175);//tamaño y coordenadas de los arcos
  
  fill(255);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(100, 105,20, 13);//tamaño y coordenadas de la elipse
  
 fill(0);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(330, 260,50, 30);//tamaño y coordenadas de la elipse
  
  point(375,265);//coordenadas de un punto
  strokeWeight(3);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(370, 270, 320, 317);//tamaño y coordenadas de la línea
  
  fill(255);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(285, 300,60, 30);//tamaño y coordenadas de la elipse
  
 strokeWeight(5);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(10, 440, 10, 490);//tamaño y coordenadas de la línea
  
   strokeWeight(5);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(60, 490, 7, 490);//tamaño y coordenadas de la línea
  
   point(70,490);//coordenadas de un punto
   point(80,490);//coordenadas de un punto
  point(90,490);//coordenadas de un punto
  
   stroke(0); //color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(0); //color del rectangulo
  rect(140, 400, 30, 90); //tamaño y coordenadas del rectangulo
  
  
   stroke(0); //color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(0); //color del rectangulo
  rect(140, 460, 100, 30); //tamaño y coordenadas del rectangulo
  
   stroke(0); //color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(255, 121, 10); //color del rectangulo
  rect(200, 360, 20, 90); //tamaño y coordenadas del rectangulo
  
  fill(255, 121, 10);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(70, 450,70, 50);//tamaño y coordenadas de la elipse
  
  
   stroke(255, 251, 10);//color del contorno
  strokeWeight(20);//tamaño del grosor del contorno
  fill(255);//color del relleno de la figura
  arc(20 ,420,200,70 ,180, 360);//tamaño y coordenadas de los arcos
  
  fill(255);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(365, 300,15, 15);//tamaño y coordenadas de la elipse
  
     strokeWeight(25);//tamaño del grosor del contorno
 stroke(255, 251, 10);//color del contorno
 line(320, 160, 400, 225);//tamaño y coordenadas de la línea
  
  strokeWeight(10);//tamaño del grosor del contorno
 stroke(5, 34, 171);//color del contorno
 line(440, 230, 420, 270);//tamaño y coordenadas de la línea
  
  stroke(0);//color del contorno
  strokeWeight(3); //tamaño del grosor del contorno
  fill(5, 34, 171); //color del rectangulo
  rect(240, 380, 110, 50); //tamaño y coordenadas del rectangulo
  
   strokeWeight(10);//tamaño del grosor del contorno
 stroke(0);//color del contorno
 line(300, 370, 420, 340);//tamaño y coordenadas de la línea
  
  
  fill(255);//color del relleno de la figura
stroke(0);//color del contorno
strokeWeight(3);//tamaño del grosor del contorno
ellipse(390, 375,25, 25);//tamaño y coordenadas de la elipse

}

# Link p5.js editable 
https://editor.p5js.org/benjaminavila2/sketches/-8ABEF4Yv
