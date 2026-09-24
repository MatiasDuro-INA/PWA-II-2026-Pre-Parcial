# Ejercicio: Detalle de Producto — de HTML a React

## Objetivo

Pasar la pantalla de detalle de producto de [product-vanilla.html](./product-vanilla.html), hecha en HTML, CSS y JavaScript puro, a componentes de React.

Abrí el archivo en el navegador y probalo antes de empezar:
- Los botones `-` y `+` cambian la cantidad.
- **Agregar al carrito** suma la cantidad elegida al contador del carrito.
- **Comprar** muestra un resumen con el producto, la cantidad y el total.

## Consignas

Resolvé los puntos en orden. Van de más fácil a más difícil.

1. **Crear la estructura.** Creá el archivo `ProductDetailReact.jsx` con un componente `ProductDetailReact` que devuelva el HTML del producto convertido a JSX. Todavía no hace falta que funcione nada. Mostralo en `App.js`.

2. **Pasar los estilos.** Importa el CSS en el componente. Acordate de cambiar `class` por `className`.

3. **Pasarle los datos desde App** Revisar que en App esta el objeto de Producto

4. **Manejar la cantidad con estado.** Usá `useState` para la cantidad y hacé funcionar los botones `-` y `+`. La cantidad no puede bajar de 1.

5. **Contador del carrito.** Agregá un estado `enCarrito` que empiece en 0. Al hacer clic en **Agregar al carrito**, sumale la cantidad elegida y mostralo arriba (🛒 Carrito: N).


6. **Componentizar el botón de agregar al carrito.** Creá el componente `BotonAgregarAlCarrito` en su propio archivo. Tiene que recibir la prop `titulo` y mostrarla como texto del botón. Usalo en `ProductDetailReact`:
   ```jsx
   <BotonAgregarAlCarrito titulo="Agregar al carrito" />
   ```

7. **Componentizar el botón de comprar.** Hacé lo mismo con `BotonComprar`, que también recibe la prop `titulo`:
   ```jsx
   <BotonComprar titulo="Comprar" />
   ```

8. **Que los botones componentizados funcionen.** Después de los puntos 6 y 7, los botones se ven pero ya no hacen nada. Hacé que vuelvan a funcionar sin mover el estado adentro de los botones. Pista: además del `titulo`, se les puede pasar una función por props.

