# Reset CSS

Este documento proporciona una referencia para un conjunto de estilos CSS de reinicio (reset) que ayuda a eliminar las inconsistencias predeterminadas de los navegadores y establecer un estilo base común para tu proyecto web.

## Estilos de Reinicio

```css
*,
html,
body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    user-select: none;
    scroll-behavior: smooth;
    list-style: none;
    font-family: var(--webkit-typography-root);
    color: var(--cl-id-00);
    cursor: default;
    text-decoration: none;
    background-repeat: no-repeat;
    background-size: cover;
    background: none;
    border: 0 none;
    outline: 0 none;
}

*::before,
*::after {
    width: 100%;
    display: block;
    position: absolute;
}

body {
    min-height: 200vh;
}

figure {
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

img {
    height: 100%;
    width: 100%;
    display: block;
    object-fit: cover;
}

svg {
    display: flex;
    justify-content: center;
    align-items: center;
}

input {
    display: flex;
    justify-content: center;
    align-items: center;

    &::placeholder {
        color: inherit;
    }
}
```

## Variables CSS (Root)

Además del reset, se definen algunas variables CSS en la raíz que facilitan la personalización de fuentes y colores en todo el proyecto.

```css
:root {
    --webkit-typography-root: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    --webkit-typography-proxyroot: ;
    --webkit-cl-id-00: ;
    --webkit-cl-id-01: ;
    --webkit-cl-id-02: ;
    --webkit-cl-id-04: ;
    --webkit-cl-id-03: ;
}
```

## Uso

Para utilizar este reset CSS en tu proyecto:

1. Copia y pega el bloque de estilos de reinicio en tu archivo CSS.
2. Define las variables CSS en el bloque `:root` según sea necesario para tu diseño.
3. Ajusta las propiedades y valores a medida que desarrollas tu sitio web.

## Notas

- Este reset CSS está diseñado para proporcionar una base sólida y neutral, permitiendo que el diseño de tu sitio web se desarrolle sobre ella.
- Asegúrate de revisar y modificar las variables según la paleta de colores y la tipografía que desees utilizar.
