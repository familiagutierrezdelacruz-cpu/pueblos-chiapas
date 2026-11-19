# 🎲 Pueblos de Chiapas

Juego de mesa tipo Monopolio con pueblos de Chiapas. Un solo archivo (`index.html`), sin servidor ni base de datos.

- Partida clásica, exprés (20 rondas) y campaña con jefes
- 2 a 4 jugadores (contra la computadora o en el mismo dispositivo)
- Insignias, retos diarios, temporadas y guardado de partida (en el navegador)

## Probar en local
Abre `index.html` en el navegador, o:

    python3 -m http.server 8000

y entra a http://localhost:8000

## Publicar
- **GitHub Pages:** se publica solo con cada `git push` a `main` (ver `.github/workflows/pages.yml`).
- **VPS:** `scp index.html usuario@IP:/var/www/pueblos/`

## Notas
Los avances, insignias y partida guardada viven en el `localStorage` de cada navegador.
