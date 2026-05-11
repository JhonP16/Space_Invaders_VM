# Space Invaders - Versión Mejorada

Este proyecto es una versión personalizada y mejorada del clásico juego Space Invaders, desarrollado en el lenguaje Jack para la plataforma Nand2Tetris.

## Características Originales
- Movimiento lateral de la nave (Rocket).
- Disparos básicos.
- Enemigos en formación de cuadrícula.
- Detección de colisiones simple.

## Mejoras Implementadas (Nuevas)

### 1. Sistema de Disparos Múltiples
Originalmente, el juego solo permitía una bala en pantalla a la vez. Hemos mejorado esto para permitir hasta **5 balas simultáneas**. Esto se logró mediante:
- Un arreglo de objetos `Bullet`.
- Lógica de gestión de balas para reutilizar balas inactivas.

### 2. Generación Aleatoria de Enemigos
Se eliminó la formación estática en cuadrícula por un sistema más dinámico:
- Implementación de un generador de números pseudoaleatorios (`Random.jack`).
- Los enemigos aparecen en coordenadas X aleatorias y diferentes alturas iniciales, creando un efecto de "lluvia de bloques".

### 3. Mecánica de Reaparición Continua (Modo Infinito)
Para aumentar la jugabilidad, los enemigos ahora son infinitos:
- Cuando un enemigo es destruido o llega al final de la pantalla, reaparece inmediatamente en la parte superior en una posición aleatoria.
- El juego se convierte en un desafío de resistencia por puntuación.

### 4. Ajustes de Dificultad
Para equilibrar la experiencia:
- Se redujo el número de enemigos activos simultáneamente a 10.
- Se aumentó la velocidad de las balas.
- Se ajustó la velocidad de descenso de los enemigos.

## Cómo Jugar
- **Flechas Izquierda/Derecha**: Mover la nave.
- **Barra Espaciadora**: Disparar (puedes disparar ráfagas de hasta 5 balas).
- **Objetivo**: Obtener la mayor puntuación posible evitando que los bloques choquen con tu nave.

---
**Desarrollado como parte del proyecto final de arquitectura de computadores.**
