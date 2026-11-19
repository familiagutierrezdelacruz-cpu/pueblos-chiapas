# 🎲 Pueblos de Chiapas

Juego de mesa tipo Monopolio con pueblos de Chiapas. App web instalable (PWA), sin servidor ni base de datos.

- Partida clásica, exprés (20 rondas) y campaña con jefes
- 2 a 4 jugadores (contra la computadora o en el mismo dispositivo)
- Insignias, retos diarios, temporadas y guardado de partida (en el navegador)
- Se instala en el celular y abre sin internet

## Archivos
- `index.html`: el juego completo
- `manifest.webmanifest`, `sw.js`, `icons/`: instalación y modo sin conexión

## Probar en local
    python3 -m http.server 8000
y entra a http://localhost:8000 (el service worker requiere http://localhost o https).

## Publicar
- **GitHub Pages:** automático con cada `git push` a `main`.
- **VPS:** `cd /var/www/pueblos && git pull`

## Notas
Avances, insignias y partida guardada viven en el `localStorage` de cada navegador.
Al cambiar `sw.js` de forma importante, sube el número de `V` (pueblos-v1 → v2) para renovar la copia guardada.
