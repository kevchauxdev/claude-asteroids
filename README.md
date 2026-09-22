# Asteroids

Clon del clásico arcade **Asteroids** implementado en canvas HTML5 puro, sin dependencias ni bundler.

## Instrucciones

- El objetivo del juego es destruir todos los asteroides para avanzar al siguiente nivel.
- Gira la nave con las flechas izquierda y derecha, impulsa con la flecha arriba y dispara con la barra espaciadora.
- Los asteroides grandes se parten en asteroides medianos, y estos en pequeños cuando reciben impacto.
- Cada asteroide tiene un valor en puntos: grande = 20, mediano = 50, pequeño = 100.
- Si chocas contra un asteroide pierdes una vida. Tienes 3 vidas en total.
- Al perder una vida, la nave reaparece con una breve invulnerabilidad para recuperar el control.
- Cuando el juego termina, presiona la barra espaciadora para reiniciar.

## Demo:

[Asteroids demo](https://klerith.github.io/claude-asteroids/)

## Descripción del juego

Nave espacial en un campo de asteroides con envolvimiento de bordes (el espacio es toroidal). Destruye asteroides para sumar puntos: los grandes se parten en medianos, los medianos en pequeños. Incluye power-ups especiales y tipos de asteroides únicos como la estrella fugaz...

## Tecnologías

- **HTML5 Canvas** — renderizado 2D
- **JavaScript (ES6+)** — lógica del juego en un solo archivo `game.js`
- Sin frameworks, sin bundler, sin dependencias

## Cómo correr

Abre `index.html` directamente en el navegador (doble clic), o usa un servidor local:

```bash
npx serve .
```

Luego visita `http://localhost:3000`.

## Controles

| Tecla     | Acción     |
| --------- | ---------- |
| `←` `→`   | Rotar nave |
| `↑`       | Propulsar  |
| `Espacio` | Disparar   |

## Puntuación

| Asteroide | Puntos |
| --------- | ------ |
| Grande    | 20     |
| Mediano   | 50     |
| Pequeño   | 100    |

## Características

- 3 vidas con invencibilidad temporal al reaparecer (parpadeo)
- Asteroides se parten en fragmentos más pequeños al ser destruidos
- Partículas de explosión al destruir asteroides
