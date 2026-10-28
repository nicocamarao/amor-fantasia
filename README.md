# AMOR · El jardín de los ocho

Prototipo local de juego 3D en HTML, CSS y JavaScript. Experiencia conceptual, no oficial ni afiliada a AMOR.

## Abrir

Abrí `index.html` en un navegador moderno. Para cargar las texturas de producto sin restricciones de archivos locales, se recomienda servir esta carpeta:

```sh
python3 -m http.server 8080
```

Luego visitá http://localhost:8080. Three.js está incluido localmente; las fuentes web son opcionales y tienen reemplazos locales. Al abrir con file://, las cajas usan etiquetas de respaldo si el navegador bloquea las texturas.

## Jugar

- Controles táctiles: tocá el jardín para caminar; la cámara sigue al personaje. También admite clic con mouse.
- Clic en una caja o un espacio pendiente del inventario para acercarte a esa variedad.
- Cerca de una caja, tocá Recolectar. La imagen aparece en un globo grande y luego viaja a su casilla del inventario.
- Esquivá los cuatro obstáculos móviles: pañal, noche sin dormir, visita de la suegra y juguetes.
- La barra de energía flota sobre el personaje. Los choques consumen energía; el tiempo y las recolecciones la recuperan. Agotarla te devuelve al inicio sin perder objetos.
- Reuní las ocho variedades, tocá Ir al cofre y luego Abrir el cofre.
- La recompensa incluye una escena romántica estilizada entre dos personajes adultos y un logro virtual sin valor comercial.
- La colección se guarda en localStorage. Reiniciá desde el botón ?.

## Fuentes

Nombres e imágenes de producto: https://preservativosamor.com/ (consultado el 28 de octubre de 2026).
Las marcas y fotografías pertenecen a sus respectivos titulares. Los escenarios, obstáculos, envases de respaldo y la recompensa son elementos ficticios del prototipo. No se realizan compras ni se ofrecen premios reales.

Three.js r158, MIT: https://github.com/mrdoob/three.js/blob/r158/LICENSE

## Vista táctil (versión 2)

Mundo 3D a pantalla completa bajo el encabezado fijo, sin desplazamiento de la página. Cámara cercana que sigue al personaje, diseño adaptable a teléfono, inventario inferior y animación de recolección. Los diálogos pueden desplazarse internamente para mantener accesible su contenido en pantallas pequeñas.

La versión anterior está respaldada en `../backups/amor-fantasia-v1-20261028-204745/`; se verificó que los 15 archivos fueran idénticos antes de editar.
