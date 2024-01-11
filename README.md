 
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