# Randomizador TikTok

Página web con una ruleta que sortea uno de 13 enlaces de TikTok y muestra un botón para abrirlo.

En la página el título es **Randomizador TikTok**. La pestaña del navegador dice **Randomizador de TikToks**. El repositorio pasó de llamarse `Ruleta-TikTok-Juego-De-Perros` a `ruleta-tiktok-perros`.

## Cómo funciona

La página completa está en `juego.html`: el marcado, los estilos y el programa van en ese mismo archivo.

1. Haz clic en **¡Girar Ruleta!**. El botón queda desactivado mientras dura el giro.
2. El programa elige un enlace al azar del arreglo `tiktokLinks`. Ahí hay 13 enlaces cortos de TikTok (`vt.tiktok.com`).
3. La ruleta gira cinco vueltas completas más un ángulo extra al azar. La animación dura 4 segundos y cada giro nuevo sigue desde el ángulo en el que se quedó.
4. Al terminar, aparece **Abrir TikTok Seleccionado**. Ese enlace abre el TikTok en una pestaña nueva.
5. **Volver a Girar** oculta el resultado y lanza otro sorteo de inmediato.

La ruleta es un círculo de 13 franjas de color, sin texto, alternadas entre rosa y cian, con una aguja fija arriba. Esa animación acompaña el sorteo. El enlace que se abre es el que salió del arreglo al empezar el giro.

Para usar otros enlaces, reemplaza las direcciones dentro de `tiktokLinks` en `juego.html` y vuelve a abrir el archivo.

## Características

- Lista fija de 13 enlaces de TikTok, escrita en el propio archivo.
- Sorteo con `Math.random()` en el navegador.
- Ruleta animada con CSS: mínimo cinco vueltas y una transición de 4 segundos.
- El botón de giro se bloquea durante la animación.
- Resultado con el texto **Abrir TikTok Seleccionado**, que abre el enlace en otra pestaña (`target="_blank"` y `rel="noopener noreferrer"`).
- Botón **Volver a Girar**, que arranca un sorteo nuevo al momento.
- Textos de la interfaz en español.
- Fondo oscuro en degradado, tarjeta centrada con desenfoque y paleta rosa (`#ff0050`) y cian (`#00f2fe` y `#25f4ee`).
- Contenedor que usa el ancho de la pantalla hasta 450 px, con viewport configurado para el celular.

## Tecnologías

- HTML5
- CSS3: Flexbox, `conic-gradient`, transiciones y `backdrop-filter`
- JavaScript del navegador, sin librerías ni frameworks
- Tipografía del sistema: Segoe UI, Tahoma, Geneva, Verdana y sans-serif

Se abre directo en el navegador: HTML, CSS y JavaScript en un solo archivo, sin paquetes que instalar.

## Cómo ejecutarlo

1. Clona el repositorio y entra a la carpeta:

```bash
git clone https://github.com/Scorpwik/ruleta-tiktok-perros.git
cd ruleta-tiktok-perros
```

2. Abre `juego.html` en tu navegador.

Desde la terminal:

```bash
xdg-open juego.html   # Linux
open juego.html       # macOS
start juego.html      # Windows
```

Listo: haz clic en **¡Girar Ruleta!** y abre el TikTok que salga.

## Autor

**Joshua Lozada** ([Scorpwik](https://github.com/Scorpwik))
