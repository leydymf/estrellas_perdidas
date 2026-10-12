# Estrellas perdidas

Videojuego de plataformas en 3D hecho en Unity. El personaje recorre el nivel recogiendo pinturas que cambian el color del mundo: según el color activo, plataformas y objetos se vuelven sólidos o se pueden atravesar, y hay que combinar los colores para avanzar.

> **English summary:** 3D platformer built in Unity 6 (C#). Collecting paint changes the world's color, and objects react to it by becoming solid or passable, so color becomes the core puzzle mechanic. Includes portals, ladders, patrolling enemies with weak points, a lives system with health pickups, respawn and game-over screens. Team project for a multimedia development course.

**Curso:** Desarrollo de Multimedia, UNAB, 2025
**Tecnologías:** Unity 6 (6000.0.47f1), C#, Input System, TextMesh Pro

## Equipo

- **Isabel Vargas:** mecánica de cambio de colores, y diseño y modelado del personaje.
- **Leydy Yohana Macareo Fuentes:** construcción del nivel y las demás mecánicas: enemigos, portales, escaleras, sistema de vidas, reaparición e interfaz.

## Mecánicas

- **Colores:** las pinturas recogidas cambian el color del fondo; los objetos se suscriben a ese cambio y activan o desactivan su colisión según el color.
- **Portales:** teletransportan al personaje a otra zona del nivel.
- **Escaleras:** el personaje detecta la escalera, sube y sale con un pequeño impulso.
- **Enemigos:** patrullan entre dos puntos y se vencen saltando sobre su punto débil.
- **Vidas:** el personaje pierde vidas al caer o tocar enemigos y las recupera con girasoles; al perderlas todas aparece la pantalla de fin de juego.

## Estructura

```
Assets/
  Character/                 Personaje, cámara, vidas, reaparición y pantallas
    Enemigo/                 Movimiento y punto débil de los enemigos
    MecanicaEscaleras/       Detección de escaleras
    MecanicasColores/        Cambio de color, objetos reactivos, pinturas y portales
  Scenes/SampleScene.unity   Nivel del juego
```

## Cómo abrirlo

Abrir la carpeta del proyecto con Unity Hub usando la versión 6000.0.47f1, cargar `Assets/Scenes/SampleScene.unity` y darle Play.
