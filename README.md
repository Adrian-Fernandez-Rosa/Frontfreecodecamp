 
  # paso 5
    Es hora de agregar algo de contenido al menú. Agregue un elemento principal dentro del elemento del cuerpo existente. Eventualmente contendrá información sobre los precios del café y los postres que ofrece la cafetería.
     <main>
      </main>


 ```html 
 <main>
</main>
 
 ```
 
# Paso 6:

El nombre de la cafetería es CAMPER CAFE. Agrega un elemento h1 dentro de tu elemento principal. Dale el nombre del café en letras mayúsculas para que se destaque.

# paso 7:

Para que los visitantes sepan que el café se fundó en 2020, agregue un elemento p debajo del elemento h1 con el texto Est. 2020.

# paso 8:

Habrá dos secciones en la carta, una de cafés y otra de postres. Agrega un elemento de sección dentro del elemento principal para que tengas un lugar para colocar todos los cafés disponibles.

```html
 <main>
      <h1>CAMPER CAFE</h1>
      <p>Est. 2020</p>
      <section>
        </section>
    </main>

```

# paso 9

Crea un elemento h2 en el elemento de sección y asígnale el texto Café.

# paso 10
Hasta ahora, has estado limitado en cuanto a la presentación y apariencia del contenido que creas. Para comenzar a tomar el control, agregue un elemento de estilo dentro del elemento principal.

# paso 11


Puede agregar estilo a un elemento especificándolo en el elemento de estilo y estableciendo una propiedad como esta:
```css
elemento {
  El valor de la propiedad;
}
```
Centre su elemento h1 estableciendo su propiedad de alineación de texto en el centro de valor.
​
```css
 <style>

      h1 {
        text-align: center;
      }
    </style>
```

# paso 12

En el paso anterior, utilizó un selector de tipo para diseñar el elemento h1. Centre los elementos h2 y p agregando un nuevo selector de tipo para cada uno al elemento de estilo existente.

```css 
<style>
      h1 {
        text-align: center;
      }
      h2{
        text-align: center;
      }
      p {
        text-align:center;
      }
 </style>
```

# paso 13

Ahora tienes tres selectores de tipo con exactamente el mismo estilo. Puedes agregar el mismo grupo de estilos a muchos elementos creando una lista de selectores. Cada selector está separado por comas como esta:

selector1, selector2 {
   El valor de la propiedad;
}
Elimine los tres selectores de tipo existentes y reemplácelos con una lista de selectores que centre el texto para los elementos h1, h2 y p.

# paso 14

Comience reescribiendo los estilos que ha creado en el archivo estilos.css. Asegúrese de excluir las etiquetas de estilo de apertura y cierre.

# paso 16

vincular archivo styles.css

# Paso 17

Para que el estilo de la página se vea similar en un dispositivo móvil al de una computadora de escritorio o portátil, debe agregar un metaelemento con un atributo de contenido especial.

Agregue lo siguiente dentro del elemento principal:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

```

# paso 18, 19

El texto se centra nuevamente para que el enlace al archivo CSS funcione. Agregue otro estilo al archivo que cambie la propiedad de color de fondo a burlywood para el elemento del cuerpo.

```css 
body {
  background-color: burlywood;
}
```

# paso 20

El elemento div se utiliza principalmente para fines de diseño, a diferencia de los otros elementos de contenido que ha utilizado hasta ahora. Agregue un elemento div dentro del elemento del cuerpo y luego mueva todos los demás elementos dentro del nuevo div.

Dentro de la etiqueta div de apertura, agregue el atributo id con un valor de menú.

```html

<body>
    <div id="menu">
        <main>
      <h1>CAMPER CAFE</h1>
      <p>Est. 2020</p>
      <section>
        <h2>Coffee</h2>
      </section>
       </main>
    </div>
  </body>
```

# Paso 21
El objetivo ahora es hacer que el div no ocupe todo el ancho de la página. La propiedad de ancho de CSS es perfecta para esto.

Puede utilizar el selector de identificación para apuntar a un elemento específico con un atributo de identificación. Un selector de identificación se define colocando el símbolo hash # directamente delante del valor de identificación del elemento. Por ejemplo, si un elemento tiene la identificación de gato, entonces apuntaría a ese elemento de esta manera:

#cat {
   ancho: 250 px;
}
Utilice el selector de menú # para darle a su elemento un ancho de 300 px.

# Paso 23
Ahora use el selector de menú # existente para establecer el color de fondo del elemento div en burlywood.

Archivo styles.css

```css
body {
  /*
  background-color: burlywood;
  */
}

h1, h2, p {
  text-align: center;
}

#menu {
  width: 300px;
  background-color: burlywood;
}
```

# Paso 24
Ahora es fácil ver que el texto está centrado dentro del elemento #menu. Actualmente, el ancho del elemento #menu se especifica en píxeles (px).

Cambie el valor de la propiedad de ancho para que sea 80%, para que sea el 80% del ancho de su elemento padre (cuerpo).

```css
#menu {
  width: 80%;
  background-color: burlywood;

}
```

# Paso 25
A continuación, desea centrar el #menú horizontalmente. Puede hacer esto configurando sus propiedades de margen izquierdo y margen derecho en automático. Piense en el margen como un espacio invisible alrededor de un elemento. Usando estas dos propiedades de margen, centre el elemento #menu dentro del elemento del cuerpo.

```css

#menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
}
```


# Paso 26
Hasta ahora has estado usando selectores de tipo e ID para diseñar elementos. Sin embargo, es más común utilizar un selector diferente para diseñar sus elementos.

Un selector de clase se define mediante un nombre con un punto directamente delante, como este:

.nombre de la clase {
   estilos
}
<p>
Cambie el selector de #menú existente a un selector de clase reemplazando #menu con una clase denominada .menu.
</p>

# paso 27

Para aplicar el estilo de la clase al elemento div, elimine el atributo id y agregue un atributo de clase a la etiqueta de apertura del elemento div. Asegúrese de establecer el valor de clase en el menú.

# Paso 28

Dado que el principal producto a la venta de la cafetería es el café, puedes utilizar una imagen de granos de café como fondo de la página.

Elimina el comentario y su contenido dentro del selector de tipo de cuerpo. Ahora agregue una propiedad de imagen de fondo y establezca su valor en url (https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg).

```css

body {
 background-image: url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg)
}
```

# paso 29

Tiene buena pinta. Es hora de comenzar a agregar algunos elementos del menú. Agregue un elemento de artículo vacío debajo del encabezado Café. Contendrá un sabor y precio de cada café que ofreces actualmente.

# paso 30

Paso 30
Los elementos del artículo suelen contener varios elementos que tienen información relacionada. En este caso contendrá un sabor a café y un precio por ese sabor. Anida dos elementos p dentro del elemento de tu artículo. El texto del primero debe ser French Vanilla y el del segundo 3.00.

```css
<article>
            <p>French Vanilla</p><p>3.00</p>
          </article>
```
# Paso 31

Comenzando debajo del par café/precio existente, agregue el siguiente café y precios usando elementos de artículo con dos elementos p anidados dentro de cada uno. Como antes, el texto del primer elemento p debe contener el sabor del café y el texto del segundo elemento p debe contener el precio.

```css
           <article>
            <p>French Vanilla</p><p>3.00</p>
</article>
           <article>  <p>Caramel Macchiato</p> <p>3.75</p> </article>
  <article>  <p>Pumpkin Spice</p> <p>3.50</p>   <article>
    <article> <p>Hazelnut</p> <p>4.00</p>   </article>
      <article> <p>Mocha </p><p>4.50</p>   </article>
```

# Paso 32
Los sabores y precios actualmente están apilados uno encima del otro y centrados con sus respectivos elementos p. Sería bueno si el sabor estuviera a la izquierda y el precio a la derecha.

Add the class name flavor to the French Vanilla p element.

```css 
 <p class="flavor">French Vanilla</p>
            <p>3.00</p>
```

# Paso 33
Usando su nueva clase flavor de tipo como selector, establezca el valor de la propiedad de alineación de texto a la izquierda.

```css
.flavor {
  text-align: left;
}
```

# Paso 34
A continuación, desea alinear el precio a la derecha. Agregue una clase llamada precio a su elemento p que tenga 3.00 como texto.

```css
 <p class="price">3.00</p>
```

# Paso 35
Ahora alinee el texto a la derecha para los elementos con la clase de precio.

```css
.price {
  text-align: right;
}
```

# Paso 36
Eso es más o menos lo que quieres, pero ahora sería bueno si el sabor y el precio estuvieran en la misma línea. Los elementos p son elementos a nivel de bloque, por lo que ocupan todo el ancho de su elemento principal.

Para colocarlos en la misma línea, debes aplicar algo de estilo a los elementos p para que se comporten más como elementos en línea. Para hacerlo, comience agregando un atributo de clase con el elemento de valor al primer elemento del artículo bajo el encabezado Café.

To do that, start by adding a class attribute with the value item to the first article element under the Coffee heading.

```html
 <h2>Coffee</h2>
          <article class="item">
            <p class="flavor">French Vanilla</p>
            <p class="price">3.00</p>
          </article>
```


# Paso 37
Los elementos p están anidados en un elemento de artículo con el atributo de clase de artículo. Puede diseñar todos los elementos p anidados en cualquier lugar de elementos con una clase denominada elemento de esta manera:

.item p { }
Usando el selector anterior, agregue una propiedad de visualización con valor inline-block para que los elementos p se comporten más como elementos en línea

```css 
.item p {
  display: inline-block;
}

```

# Paso 38
Eso está más cerca, pero el precio no se quedó a la derecha. Esto se debe a que los elementos de bloque en línea solo ocupan el ancho de su contenido. Para distribuirlos, agregue una propiedad de ancho a los selectores de clase de sabor y precio que tienen un valor del 50% cada uno.

```css 
.flavor {
  text-align: left;
   width: 50%;
}

.price {
  text-align: right;
    width: 50%;
}
```


# Paso 39

Bueno, eso no funcionó. Diseñar los elementos p como bloques en línea y colocarlos en líneas separadas en el código crea un espacio adicional a la derecha del primer elemento p, lo que hace que el segundo se desplace a la siguiente línea. Una forma de solucionar este problema es hacer que el ancho de cada elemento p sea un poco menos del 50%.

Cambie el valor del ancho al 49% para cada clase para ver qué sucede.

```css 
.flavor {
  text-align: left;
  width: 49%;
}

.price {
  text-align: right;
  width: 49%;
}
```

# Paso 40
Eso funcionó, pero todavía hay un pequeño espacio a la derecha del precio.

Podrías seguir probando varios porcentajes para los anchos. En su lugar, use la tecla de retroceso en su teclado para mover el elemento p con el precio de clase al lado del elemento p con el tipo de clase para que estén en la misma línea en el editor. Asegúrate de que no haya espacio entre ellos.

```css 
<p class="flavor">French Vanilla</p><p class="price">3.00</p>
```

# Paso 41
Ahora continúe y cambie el ancho de la clase de sabor y de precio para que vuelva a ser del 50 %.


# Paso 42

Ahora que sabes que funciona, puedes cambiar el artículo restante y los elementos p para que coincidan con el primer conjunto. Comience agregando el elemento de clase a los otros elementos del artículo.

code index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cafe Menu</title>
    <link href="styles.css" rel="stylesheet"/>
  </head>
  <body>
    <div class="menu">
      <main>
        <h1>CAMPER CAFE</h1>
        <p>Est. 2020</p>
        <section>
          <h2>Coffee</h2>
          <article class="item">
            <p class="flavor">French Vanilla</p><p class="price">3.00</p>
          </article>
          <article class="item">
            <p class="flavor">Caramel Macchiato</p>
            <p class="price">3.75</p>
          </article>
          <article class="item">
            <p class="flavor">Pumpkin Spice</p>
            <p class="price">3.50</p>
          </article>
          <article class="item">
            <p class="flavor">Hazelnut</p>
            <p class="price">4.00</p>
          </article>
          <article class="item">
            <p class="flavor">Mocha</p>
            <p class="price">4.50</p>
          </article>
        </section>
      </main>
    </div>
  </body>
</html>

```

style.css

```css
body {
  background-image: url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg);
}

h1, h2, p {
  text-align: center;
}

.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
}

.item p {
  display: inline-block;
}

.flavor {
  text-align: left;
  width: 50%;
}

.price {
  text-align: right;
  width: 50%;
}
```

# Paso 43
A continuación, coloque los otros p elementos para que estén en la misma línea sin espacios entre ellos.
​

```html

  <article class="item">
            <p>Caramel Macchiato</p><p>3.75</p>
          </article>
          <article class="item">
            <p>Pumpkin Spice</p><p>3.50</p>
          </article>
          <article class="item">
            <p>Hazelnut</p><p>4.00</p>
          </article>
          <article class="item">
            <p>Mocha</p><p>4.50</p>
          </article>
```

# Paso 44
Para completar el estilo, agregue el sabor y el precio de los nombres de clase aplicables a todos los elementos p restantes.

# Paso 45
Si reduce el ancho de la vista previa de la página, notará que en algún momento parte del texto de la izquierda comienza a pasar a la siguiente línea. Esto se debe a que el ancho de los elementos p en el lado izquierdo solo puede ocupar el 50% del espacio.

Como sabe que los precios de la derecha tienen muchos menos caracteres, cambie el valor del ancho de la clase de sabor para que sea 75 % y el valor del ancho de la clase de precio para que sea 25 %.

```css
.flavor {
  text-align: left;
  width: 75%;
}

.price {
  text-align: right;
  width: 25%;
}
```

# Paso 46
Volverá a diseñar el menú en unos pocos pasos, pero por ahora, continúe y agregue un segundo elemento de sección debajo del primero para mostrar los postres que ofrece la cafetería.

# Step 47
Add an h2 element in the new section and give it the text Desserts.

```css
<section>
          <h2>Desserts</h2>
</section>
```

# paso 48
Agregue un elemento de artículo vacío debajo del encabezado Postres. Dale un atributo de clase con el elemento de valor.

```html
<h2>Desserts</h2>
          <article class="item"> </article>
```


# paso 49
Nest two p elements inside your article element. The first one's text should be Donut, and the second's text 1.50. Put both of them on the same line making sure there is no space between them.

```html
   <article class="item">
            <p>Donut</p><p>1.50</p>
          </article>
```

# Paso 50
Para los dos elementos p que acaba de agregar, agregue postre como el valor del atributo de clase del primer elemento p y el valor del precio como atributo de clase del segundo elemento p.

```html
<p class="dessert">Donut</p><p class="price">1.50</p>
```

# Paso 51
Algo no parece correcto. Agregó el valor de atributo de clase correcto al elemento p con Donut como texto, pero no definió un selector para él.

La regla CSS para la clase de tipo ya establece las propiedades que desea. Agregue la clase dessert como selector adicional para esta regla CSS.

```css
.flavor , .dessert {
  text-align: left;
  width: 75%;
}

```


Paso 52
Debajo del postre que acaba de agregar, agregue el resto de los postres y los precios usando tres elementos de artículo más, cada uno con dos elementos p anidados. Cada elemento debe tener el texto correcto de postre y precio, y todos deben tener las clases correctas.

Cherry Pie 2.75
Cheesecake 3.00
Cinnamon Roll 2.50

```html
        <article class="item">
            <p class="dessert">Donut</p><p class="price">1.50</p>
             </article>
              <article class="item">
            <p class="dessert">Cherry Pie</p><p class="price">2.75</p>
             </article>
              <article class="item">
            <p class="dessert">Cheesecake</p><p class="price">3.00</p>
             </article>
              <article class="item">
            <p class="dessert">Cinnamon Roll</p><p class="price">2.50</p>
             </article>
```

# Paso 53
Puedes darle a tu menú algo de espacio entre el contenido y los lados con varias propiedades de padding.

Give the menu class a padding-left and a padding-right with the same value 20px.

```css
.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
  padding-left: 20px;
  padding-right: 20px;
}
```

# Step 54
That looks better. Now try to add the same 20px padding to the top and bottom of the menu.
```css
  padding-bottom: 20px;
  padding-top: 20px;

```

# Paso 55
Dado que los 4 lados del menú tienen el mismo espacio interno, continúe y elimine las cuatro propiedades y use una única propiedad de padding con el valor 20px.

```css 

padding: 20px;

```