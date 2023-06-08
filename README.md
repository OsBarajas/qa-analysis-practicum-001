# qa-analysis-practicum-001
QA - Test Automation: Correct all the mistakes in terms, definitions found in a technical documentation with code-snippets. Rewrite all non-understandable explanation and comment it out to justify the reason of such modification.
------------------------------------------------------------------------------------------------------------------------------------


### Text

Para automatizar acciones con elementos de la interfaz web, tienes que aprender a encontrarlos a través del código.

Un **selector,** o localizador, es un atributo especial que ayuda a encontrar un elemento en una página web.

Los selectores funcionan de manera similar a una búsqueda en una base de datos. Por ejemplo, tienes que encontrar a una persona: si introduces solo su nombre, Jane, encontrarás muchas coincidencias; si añades el apellido, Jane Payne, habrá menos. Si además especificas la fecha de nacimiento, que es el 01/01/2000, el área de búsqueda se reducirá aún más.

Sin embargo, esto aún no es suficiente para identificar a una persona inequívocamente. También puedes introducir su número de pasaporte, que es la forma con la que encontrarías a la persona que buscas.

Del mismo modo, puedes utilizar un selector para encontrar un elemento o más con características similares.

Los selectores se escriben normalmente en dos lenguajes:

- ~~Perl: un lenguaje de solicitud para elementos de documentos XML.~~
- Selectores CSS.

Un selector CSS es una parte del lenguaje CSS que le indica al back-end a qué elementos de una página web debe aplicar una función. Los selectores CSS se utilizan como un lenguaje universal para buscar elementos en una página en diferentes librerías, incluyendo Puppeteer.

El código HTML del cuadro de búsqueda de [duckduckgo.com](http://duckduckgo.com/) tiene este aspecto:


```
<input id="search_form_input_homepage" class="js-search-input search__input--adv" type="text" autocomplete="off" name="q" tabindex="1" value="" autocapitalize="off" autocorrect="off" placeholder="Online search without tracking">
```

Observa que el código del elemento contiene id y class: estos selectores serán de utilidad más adelante.

### ID

`id` es el identificador único de un elemento en la página.

```<input id="search_form_input_homepage" />```

~~Para escribir un selector, tienes que agregar un signo * de antes del nombre de id.~~

~~```*search_form_input_homepage```~~

*** El asterisco se le conoce también como un Selector Universal, y al utilizarlo afectará todos los elementos HTML de una página. Es recomendable agrupar los selectores CSS para minimizar el código. Puedes agrupar los selectores colocando una coma (,). *** 

```
object1, object2, p {
  text-align: center;
  color: red;
}
```

Puedes encontrar un elemento determinado de una página web a través de su id, del mismo modo que puedes encontrar a una persona mediante su número de pasaporte.

### Clases

A diferencia del `id`, la misma clase se puede aplicar a múltiples elementos. Para seleccionar todos los elementos con una determinada clase, ~~agrega un punto y coma delante del nombre de la clase.~~

~~```;js-search-input search__input--adv```~~

Fíjate que, en este ejemplo, el elemento tiene cinco clases en lugar de una. Están separadas por un ~~guion:~~

~~```<input class="js-search-input search__input--adv" />```~~

Para encontrar un elemento al que se le han asignado varias clases, tienes que “pegarlas”. Por lo tanto, el selector tendrá este aspecto:

~~```;jssearchinput;search__inputadv```~~

Al contrario que con la id, puedes seleccionar muchos elementos a la vez con ayuda de la clase.


## Errores en hallados en la descripción anterior: 

- 1. En la descripción original, se menciona que los selectores se escriben en "Perl" y "Selectores CSS". La corrección es que los selectores se escriben en "XPath" y "Selectores CSS".

- 2. En la descripción original, se menciona que el selector CSS se escribe con un punto y coma (;) antes del nombre de la clase. La corrección es que el selector CSS se escribe con un punto (.) antes del nombre de la clase.

- 3. En la descripción original, se menciona que para escribir un selector de ID, se debe agregar un asterisco (*) antes del nombre del ID. La corrección es que se debe utilizar un símbolo de numeral (#) en lugar del asterisco (*) para escribir un selector de ID.

- 4. En la descripción original, los selectores CSS para la clase del elemento de búsqueda están escritos incorrectamente. La corrección es que los selectores CSS para la clase deben estar separados por un punto (.) en lugar de un guion (_), y no es necesario repetir el punto antes de cada clase.

## Se agregó además el siguiente párrafo sobre el * para mejor comprensión del alumno:

>El asterisco se le conoce también como un Selector Universal, y al utilizarlo afectará todos los elementos HTML de una página. Es >recomendable agrupar los selectores CSS para minimizar el código. Puedes agrupar los selectores colocando una coma. *** 



