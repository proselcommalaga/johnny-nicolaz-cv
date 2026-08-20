# QA del CV público

`QA_LOCAL_VERDICT: pass`  
`QA_PUBLICATION_VERDICT: pass`

## Revisión local 2026-08-20

| Gate | Resultado | Evidencia |
| --- | --- | --- |
| Estructura | Pasa | Un `article.cv`, un dashboard, un `h1` y un pie |
| Métricas | Pasa | 15+, 7 experiencias, 4 ámbitos y 2 titulaciones; distribución 3/2/1/1 |
| Privacidad | Pasa | Sin dirección postal completa y sin métricas comerciales inventadas |
| Escritorio | Pasa | Dashboard alineado con la columna principal y la formación lateral |
| Móvil 360 px | Pasa | Una columna y sin desbordamiento horizontal |
| Teclado | Pasa | Orden inicial: saltar al contenido, teléfono, correo |
| Contraste | Pasa | Blanco/verde `6,37:1`; blanco/azul `9,44:1`; tinta/amarillo `9,06:1`; texto secundario/blanco `6,24:1` |
| Consola | Pasa | Sin errores ni advertencias en Edge |
| Movimiento reducido | Pasa | Las transiciones se desactivan con `prefers-reduced-motion` |
| Alto contraste | Pasa por código | Bordes explícitos bajo `forced-colors`; pendiente prueba con lector de pantalla real |
| Impresión | Preparado | Estilos A4 incluidos; pendiente inspección visual del PDF final si se distribuye |

## Gate después de publicar

- [x] La URL de GitHub Pages responde correctamente.
- [x] El `title`, la descripción y la URL canónica son correctos.
- [x] Se ve una sola copia del CV.
- [x] El dashboard conserva su alineación en escritorio.
- [x] A 360 px no existe desplazamiento horizontal.
- [x] El final termina después del pie del CV, sin contenido duplicado.
- [x] Teléfono y correo conservan sus enlaces.
- [x] La consola pública no presenta errores.

## Evidencia pública 2026-08-20

- URL: <https://proselcommalaga.github.io/johnny-nicolaz-cv/>
- Respuesta HTTP: `200`.
- Archivos `index.html`, `README.md` y `QA.md`: contenido normalizado idéntico al local antes de este cierre de QA.
- Edge escritorio: ancho de contenido `1897 px`, sin desbordamiento horizontal.
- Edge móvil: viewport `360 px`, ancho útil `345 px`, una columna y sin desbordamiento horizontal.
- Estructura pública: un `article.cv`, un `h1`, un dashboard, cuatro tarjetas métricas, siete experiencias y un pie.
- Consola pública: sin errores ni advertencias.

`QA_VERDICT: pass`

