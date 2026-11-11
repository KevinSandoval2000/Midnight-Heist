# Midnight Heist: Pixeland Arcade

Juego arcade de sigilo y laberintos en pixel art, hecho con **un solo archivo HTML** y **cero assets**: todo (escenarios, personajes, luces y sonido) se genera con código en el navegador.

## Jugar

Abre `index.html` en un navegador moderno, o sirve la carpeta:

```bash
python3 -m http.server 8080
```

Luego visita <http://localhost:8080>.

## Controles

- **WASD / Flechas**: mover
- **E**: esconderse / salir / abrir cajas sorpresa
- **R**: reiniciar el nivel
- **Enter**: empezar / continuar

## Mecánicas principales

- **Visibilidad limitada:** el laberinto está a oscuras. El jugador y los guardias (máximo 6 por nivel) usan linternas con conos de luz dinámicos que las paredes bloquean. Entrar en el haz de un guardia inicia una persecución.
- **Invulnerabilidad inmediata al esconderse:** si logras interactuar con un escondite (caja, barril, cuadro, etc.), te vuelves **100% indetectable e invulnerable al instante**. Aunque un guardia te esté iluminando directamente y vea cómo te escondes, cancela la persecución de inmediato, muestra un símbolo **?**, pierde el interés y vuelve a su ruta de patrulla normal. El jugador siempre se salva si logra accionar un escondite a tiempo.
- **Patrullaje independiente y constante:** cada guardia elige y recorre su propia ruta por el laberinto, con objetivos y tiempos independientes. Los guardias siguen patrullando aunque el jugador esté completamente quieto.
- **Cajas sorpresa (70/30):** cada caja tiene un **70% de probabilidad de dar un bonificador** (velocidad x2, invisibilidad temporal o guardias paralizados) y un **30% de probabilidad de dar una penalización** (controles invertidos, linterna apagada 10 segundos o alerta de ruido que atrae a los guardias).
- **Gallinas y llave:** roba las **3 gallinas blancas** para que aparezca la llave; recógela y llega a la puerta. Las **6 gallinas de oro** dan puntos extra y, si reúnes las 6, la llave y la salida brillan a través de la oscuridad.
- **Límite de tiempo:** **300 segundos** por nivel; si se agotan, la captura es automática.

## Objetivo

- Roba las 3 gallinas blancas, consigue la llave y escapa por la puerta antes de que termine el tiempo.
- Reúne las 6 gallinas de oro para activar la guía luminosa hacia la salida.

## Los 10 niveles

1. Laberinto de Neón
2. Reino Fúngico
3. Ruinas de Insectos
4. Zona de Guerra
5. Las Profundidades
6. Turno de Noche
7. Colina Verde
8. Cuadrilátero Explosivo
9. Mazmorra del Héroe
10. Glitchland (mezcla aleatoria)

## Reglas del reto

- `index.html` pesa **menos de 32 KB**.
- Sin librerías, frameworks ni motores.
- Cero assets externos: gráficos y sonido por código.
- Repositorio nuevo e idea original (homenajes temáticos, sin copiar assets ni personajes).
- **Cualquiera puede participar**, esté o no en el hackatón.

## Contribuir

Abre un issue o envía un pull request. No necesitas estar en el hackatón: mejoras de balance, nuevos temas, accesibilidad, mobile, etc. son bienvenidas. Mantén el juego en un solo archivo y por debajo de 32 KB.

## Licencia

MIT. Ver `LICENSE`.
