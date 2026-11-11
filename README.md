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

## Objetivo

- Roba las **3 gallinas blancas** para que aparezca la llave.
- Recoge la llave y llega a la puerta antes de que terminen los **300 segundos**.
- Las **6 gallinas de oro** dan puntos extra; si las reúnes todas, la llave y la salida brillan a través de la oscuridad.
- Cada nivel tiene guardias con linterna y conos de visión, escondites temáticos y 6 cajas sorpresa (50% bonus / 50% penalización).

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
