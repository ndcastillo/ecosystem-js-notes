El **estado de los datos** a lo largo del tiempo de una aplicación pueden cambiar, y se necesita un proceso **reactivo** para que toda la UI cambien en conjunto. Por ejemplo los estados de inicio de sesión:

```json
{
    user:true
}
///
{
    user:false
}
```

El **estado** serán datos que controlaran la lógica de aplicación en un momento dado, por cuanto es común escuchar *el estado actual de los datos de la aplicación*.

## Interfaces basadas en el estado

Las **interfaces basadas en el estado** se refieren a las interfaces que cambian de acuerdo al estado de los datos, como se sabe las interfaces se pueden dividir en **componentes**, y estos componentes son configurables de a cuerdo a los estados de variables.

A este paradigma se lo llama **reactividad de los datos**, y es que la interfaz de usuario se modifica de acuerdo a los cambios de los datos, esto con el objetivo de que coincida con la lógica de programación.

Las características de los componentes son:

- Es un fragmento de la interfaz que cumple una función.

- Son reutilizables.

- Son autonomos e independientes al contexto de otros componentes.

Se puede implementar la **reactividad** ya sea con frameworks como en Vanilla Javascript.

## Paradigmas

**Existen muchas formas de escribir código**, muchas opciones para llegar al mismo resultado con diferentes lógicas y estilos de programación. A estas formas de resolver y diseñar un problema se le llaman **paradigmas de programación**. Existen [4 paradigmas](https://www.cs.ucf.edu/~leavens/ComS541Fall97/hw-pages/paradigms/major.html) mas conocidos dentro de los lenguajes de programación.

1. Imperativo

2. Descriptiva

3. Funcional

4. Orientado a Objetos

### Programación Imperativo

El paradigma de programación imperativa asume que la computadora puede mantener a través de entornos de variables cualquier cambio en un proceso de cómputo. Se preocupa mas por el **que se resuelve***  y el como? lo dejamos aparte.

### Programación Descriptiva

El Paradigma Lógico o descriptivo adopta un enfoque declarativo para la resolución de problemas. Se hacen varias afirmaciones lógicas sobre una situación, estableciendo todos los hechos conocidos y detalla a groso modo la forma de solución.

### Programación Funcional

El paradigma de la programación funcional ve todos los subprogramas como funciones en una caja negra, en la cual tomara argumentos y devolverá una única solución.

### Programación Orientada a Objetos (OOP)

Es un paradigma en el cual los objetos de la vida real son vistos como entidades separadas que tienen su propio estado, y estos serán modificados a través constructores (clases) que editaran atributos y diseñaran métodos para realizar invocaciones. Algunas de sus características es que se pueden generar objetos en base a clases, y puedes generar otros objetos heredando clases y subclases.

## Paradigma de la programación Reactiva

Sabiendo que es un **paradigma de programación**, entonces decimos que la reactividad es un **paradigma**, este cumplira con dos lineamientos: ser **Reponsive** y ser **Message Driven**.

### 1. Lineamiento de Responsive

Para que cumpla que una aplicación sea responsive, esta tendrá dos características importantes que es la **resilencia** y la **escalabilidad** de una aplicación.

:::(Info) (Nota:)
Que una aplicación sea responsive nos referimos al paradigma de programación y no a la adaptabilidad de los estilos a distintas pantallas.
:::

- **Resiliente:** Significa que nuestra aplicación tiene la capacidad de adaptarse a cualquier situación, por ejemplo ante un error de cliente, error del servidor, errores del canal, etc.

- **Escalable:** Es decir que la aplicación es elástica, y puede crecer armoniosamente sin problemas.

### 2. Lineamiento de Message Driven

La arquitectura basada en mensajes o Message Driven, **se basa en emisores y receptores de mensajes**, y su caracteristica es que **los mensajes se envian asincronicamente y se guardan en una cola** a la cual los receptores deben **suscribir** para recibir los mensajes. 

Por ejemplo el emisor A envia un mensaje y el *queue agregator* o gestor de cola sabra en que cola se debe guardar ese mensaje que acaba de llegar y notifica a todos los receptores que se encuentran suscritos a esta cola en particular, que llego un nuevo mensaje.

## Estado de Variables

Estado o *state* de las variables es el lugar donde se almacena la información reactiva de los componentes. Los estados seran 

:::(Info) (PostData:)
No todas los frameworks usan el termino de estado, pero utilizan otros terminos que tienen la escencia de lo que es un estado.
:::

## Rederizado en el Navegador

Existen muchas estrategias para realizar el renderizado (pintado) en el Navegador, y es que la manipulación de los elementos del DOM son variadas, algunas buscan la optimización de recursos o la agilidad de los procesos, y dependera de la libreria o framework que estes utilizando.

### Virtual DOM

La estrategia del virtual DOM se efectuara cada vez que haya que aplicar un renderizado, aquí se hará una copia virtual del DOM inicla en Javascript (se almacenara en bancos de memoria específicos) y cuando sea necesario realizar una modificación en un componente lo hacemos directamente en el Virtual DOM.

![](img\2022-08-23-12-17-09-image.png)

De esta manera no tendremos que eliminar un nodo y crear otro nodo, cada vez que necesitemos modificar su contenido o sus propiedades. El virtual DOM se encargara de comparar la versión inicial con la modificada y únicamente cambiara en el virtual DOM.

## No Virtual DOM

Otra corriente, menciona que no hay la necesidad de generar una copia completa del DOM en Javascript, y que es un paso innecesario. Esta corriente menciona que en vez de generar un virtual DOM de todo el DOM, es preciso únicamente realizar una pequeña copia del DOM en especifico el componente que se quiere modificar, de esta manera enfocar únicamente los recursos en un componente.

![](img\2022-08-23-12-17-38-image.png)

## Resumen

Se parte por la creación de un **componente**, este tendrá ciertos atributos y **estados** que lo caracterizan, y esta expuesto al **usuario**. El usuario sera el encargado de interactuar con el componente y efectuar el cambio de estado del componente, entonces se seguirá una estrategia de **renderizado** del navegador para presentarle al usuario se presentara al usuario.

![](C:\Users\raycr\AppData\Roaming\marktext\images\2022-08-23-12-19-02-image.png)


**Contribución realizada por:** David Castillo
