# La Cherry — demo para publicación

Este paquete permite publicar una **demostración** como sitio estático.

## Publicación en Render
1. Crea un repositorio en GitHub y sube `index.html` y `render.yaml` a la raíz.
2. En Render, crea un nuevo **Static Site** conectado a ese repositorio (o usa Blueprint con render.yaml).
3. Build command: `echo 'Sitio estático listo'`.
4. Publish directory: `.`.
5. Publica y abre el dominio que Render asigne.

## Limitaciones importantes
- Los pedidos se guardan en `localStorage` del navegador: NO se comparten entre dispositivos.
- El panel administrador no tiene autenticación y NO debe usarse para recibir pedidos reales.
- Los PDF se obtienen mediante el diálogo de impresión del navegador.
- Faltan implementar pedidos adicionales con edición/cancelación, límites de horario, backend y protección de datos.

Antes de abrirlo a padres, conectar una base de datos con políticas de acceso, separar el panel administrativo y probar la operación de extremo a extremo.
