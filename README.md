# Equa

Citas que empiezan en una mesa, no en un chat.

**https://srinsolente.github.io**

Desde el móvil se puede añadir a la pantalla de inicio: se abre como una
aplicación, sin barra de navegador.

## Qué es y qué no es

Es la aplicación de verdad compilada para navegador: las mismas pantallas,
las mismas reglas y el mismo recorrido que la versión de móvil. Los perfiles
y los eventos son de ejemplo, y todo lo que hagas se guarda únicamente en tu
propio navegador. No hay servidor detrás todavía, así que nadie más ve lo que
haces aquí.

Lo único que no existe en esta versión es la biometría, que es del teléfono.

## Cómo está hecho

`index.html` es un único archivo con todo dentro: el código de las catorce
pantallas, las tipografías y los iconos. No pide nada por red. `404.html` es
una copia, para que recargar estando en una pantalla siga funcionando.

Se genera desde el proyecto con:

```
npx expo export --platform web --output-dir dist-web
node scripts/pagina-web.mjs
```

El código fuente vive aparte.
