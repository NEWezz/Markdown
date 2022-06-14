# Aprende _markdown_

![Markdown](https://comika.es/wp-content/uploads/2020/08/markdown-guide-og.jpg)

## ¿Que es markdown?

_Markdown_ es un lenguaje de marcado que facilita la aplicación de formato a un texto empleando una serie de caracteres de una forma especial. En principio, fue pensado para elaborar textos cuyo destino iba a ser la web con más rapidez y sencillez que si estuviésemos empleando directamente HTML. Y si bien ese suele ser el mejor uso que podemos darle, también podemos emplearlo para cualquier tipo de texto, independientemente de cual vaya a ser su destino.

---

Como explica "John Gruber":http://daringfireball.net/projects/markdown/, uno de sus creadores, Markdown es realmente dos cosas: por un lado, el lenguaje; por otro, una herramienta de software que convierte el lenguaje en HTML válido. Para entenderlo mejor, veámoslo con un ejemplo. Digamos que queremos escribir un encabezado de nivel 1. Esto en HTML se hace con la etiqueta h1. Por lo tanto, escribiríamos:

## Encabezados

hacer encabezados es muy facil. solo debes agregarle al principio el # segun su tipo gerargico

por ejemplo:

# encabezado de tipo 1 \#

## encabezado de tipo 2 \##

### encabezado de tipo 3 \###

#### encabezado de tipo 4 \####

##### encabezado de tipo 5 \#####

###### encabezado de tipo 6 \######

---

## Párrafos

solámente haciendo un enter y escríbiendo sin ningún caracter, ya estas creando un parrafo.

---

## _Cursiva_ y **negrita**

Para crear un texto cursiva solo debemos poner el guión bajo \_y la pálabra\_.

nos quedaria así:
_Este es un texto en cursiva_

Para crear un texto negrita solo debemos poner doble asterisco \*\*y la pálabra\*\*.

nos quedaria así:
**Este es un texto en negrita**

---

## Enlaces externos

Para poner enlaces solo debemos poner dos cosas:

1. Cochetes \[ ] _Ponemos el nombre del enlace_.
1. Parentesis \() _Ponemos la url del enlace_.

Ejemplo:

\[Nombre del enlace] (url del enlace)

Nos quedaria así

[Nombre del enlace](https://www.youtube.com/)

_Nota_: No agregar espacio entre los **corchetes** y el **parentesis**.

---

## Enlaces internos

Por default los encabezados en _Markdown_ son un enlace o una ancla interna, usted puede navegar internamente en su documentación , blog o en su temario a traves de estos encabezados.

por ejemplo volvamos al encabezado que de tipo 1 aprende _Markdown_.

con el # automaticamente aparecera para elegir que encabezado queremos para navegar internamente haciendo click en el enlace.

ejemplo:

```markdown
[aprende _markdown_](#aprende-markdown)
```

Nos quedaria así

[Aprende _markdown_](#aprende-markdown)

---

## Imagenes

las imagenes funcionan igual que los [enlaces externos](#enlaces-externos) o [enlaces externos](#enlaces-internos)

### imagen externa

```markdown
[Imagen externa](https://jonmircha.com/img/blog/this-is-javascript.jpg)
```

Nos quedaria asi

[Imagen externa](https://jonmircha.com/img/blog/this-is-javascript.jpg)

---

### Imagen interna

Para poner una imagen interna en los parentesis se le debe especificar la ruta en donde esta su imagen.

Ejemplo:

```markdown
[Imagen interna](img/oranges.png)
```

Nos quedaria así:

[Imagen interna](img/oranges.png)

Nota: Para que la imagen ya sea externa o interna se muestre en Markdown, tenemos que anteponer el ! a los corchetes

ejemplo:

\!\[aca va lo que seria el alt en html](img/oranges.png)

Nos quedaria así
![aca va lo que seria el alt en html](img/oranges.png)

---

## Tablas

Para crear tablas necesitamos de los caracteres py o | y guiones o -

### encabezado de la tabla

| Nombre | edad | Pais |

---

### Linea que separa el encabezado con los datos

```markdown
| Nombre | Edad | Pais |

| ------ | ---- | ---- |
```

Nos quedaria así:

| Nombre | Edad | Pais |
| ------ | ---- | ---- |

### Datos

```markdown
| Nombre | Edad | Pais |

| ------ | ---- | ---- |

| Ezequiel | 20 | Argentina |
```

Nos quedaria asÍ:

| Nombre   | Edad | Pais      |
| -------- | ---- | --------- |
| Ezequiel | 20   | Argentina |
| David    | 30   | Peru      |

---

## Listas

### Lista ordenada

Para crear un lista ordenada debemos ante poner 1. y espacio.

ejemplo:

```markdown
1. Primavera
1. verano
1. otoño
1. Invierno
```

Nos quedaria así:

1. Primavera
2. verano
3. otoño
4. Invierno

### Lista desordenada

para crear una lista desordenada debemos ante poner el guión medio y espacio .

ejemplo:

```markdown
- Primavera
- verano
- otoño
- Invierno
```

Nos quedaria así:

- Primavera
- verano
- otoño
- Invierno

### SubLista

Si quieres generar listas anidadas (sublistas), usa la indentación para controlar los niveles de los elementos de la lista.

ejemplo:

```markdown
- Primavera

  - Sectiembre
  - Noviembre

- verano
- otoño
- Invierno
```

Nos quedaria así:

- Primavera

  - Sectiembre
  - Noviembre

- verano
- otoño
- Invierno

---

## Códigos

Podemos dar formato de código a un texto, para ello se usa el acento grave (`).

Podemos declarar código en una sóla línea o en bloque.

### Código en línea

```markdown
Esto es `código` en línea.

En _JavaScript_ una variable se define así: `let saludo = "Hola Mundo";`.
```

### Código en bloque

````markdown
```js
function sumar(a, b) {
  if (typeof a !== "number" || typeof b !== "number") {
    console.error(`Los valores ingresados NO son números.`);
    return false;
  }

  let c = a + b;
  return c;
}
```
````

Nos quedaria así:

```js
function sumar(a, b) {
  if (typeof a !== "number" || typeof b !== "number") {
    console.error(`Los valores ingresados NO son números.`);
    return false;
  }

  let c = a + b;
  return c;
}
```

---

## Comentarios

Los comentarios son textos ignorados por el programa que interpreta o compila el código, no se visualizarán. Sirven a los programadores para dejar notas en el código. Markdown utiliza el mismo formato que _HTML_ para comentar.

```markdown
<!--Esto es un comentario-->
```

---

## Divisiones

En HTML se tiene la etiqueta `<hr>` para definir una división o ruptura semántica entre bloques de contenido. Se visualiza como una línea horizontal.

```markdown
un bloque de contenido

---

otro bloque de contenido
```

## Escaparates

Se le llama escape de caracteres al proceso que hace un lenguaje de marcado o programación para omitir los caracteres especiales que usa para la definición de su sintaxis. Al escapar caracteres, el lenguaje los interpretará como simple texto plano.

Por ejemplo Markdown usa los siguientes caracteres especiales: guión bajo, medio, asterísco, corchetes cuadrados, paréntesis, almohadilla, acento grave, barra invertida, etc.

Para escapar un caracter en Markdown sólo tenemos que anteponerle un barra invertida \\.

```markdown
Texto en \_cursiva\_ y \*\*negrita\*\*.
```

Texto en _cursiva_ y **negrita**.

---

## Citas

Podemos dar formato de cita a un texto, anteponiendo a la línea de texto un carcater de mayor qué (>).

Podemos declarar citas en una sóla línea o en bloque

### Citas en Línea

```
> Todo lo que escuchamos es una opinión, no un hecho. Todo lo que vemos es una perspectiva, no la verdad. - Marco Aurelio.
```

> Todo lo que escuchamos es una opinión, no un hecho. Todo lo que vemos es una perspectiva, no la verdad. - Marco Aurelio.

### Citas en bloque

```


> Todo lo que escuchamos es una opinión, no un hecho. Todo lo que vemos es una perspectiva, no la verdad.
>
> Marco Aurelio.
```

> Todo lo que escuchamos es una opinión, no un hecho. Todo lo que vemos es una perspectiva, no la verdad.
>
> Marco Aurelio.

---

## Aprende más

```
_cursiva_

**negrita**

~tachado~

**_cursiva y negrita_**

_~cursiva y tachado~_

**~negrita y tachado~**

**_~cursiva, negrita y tachado~_**
```

_cursiva_

**negrita**

~tachado~

**_cursiva y negrita_**

_~cursiva y tachado~_

**~negrita y tachado~**

**_~cursiva, negrita y tachado~_**
