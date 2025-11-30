# Documentación del Proyecto: (P)Resident Evil - The Moncloa Nightmare

Este directorio contiene toda la documentación de diseño, narrativa, mecánicas y especificaciones técnicas del videojuego desarrollado por **Grupo Pantumaca**.

El proyecto es un *Survival Horror* satírico con elementos RPG y de Acción ambientado en el Palacio de la Moncloa durante un apocalipsis zombi político.

---

## Índice de Documentos

Actualmente, la documentación se divide en los siguientes archivos:

### 1. [Historia y Ambientación](./historia_ambientacion.md)
*Contiene la narrativa, el perfil del protagonista y la construcción del mundo.*
* **Premisa:** Pedro Sánchez despierta en la última planta de una Moncloa corrupta y debe descender para escapar.
* **Sistema de Salud:** Explicación del "Nivel de Corrupción" que sustituye a la barra de vida tradicional.
* **Enemigos:** Descripción de los jefes (líderes internacionales como Trump o Xi Jinping), amenazas invencibles (Tribunal de Cuentas) y enemigos estándar.
* **Objetivo de Nivel:** La mecánica de encontrar el "Sobre con dinero negro" para sobornar al jefe de planta y avanzar.

### 2. [Mecánicas y Sistemas](./mecanicas.md)
*Detalla las reglas del juego, los tres géneros principales y las matemáticas detrás del combate.*
* **Acción:** Sistema de estados del enemigo (Atacar, Defender, Decretazo, Mareado).
* **RPG:** Tablas de afinidades políticas (Liberal, Conservador, Socialista) y bonificaciones de equipo.
* **Survival Horror:** Gestión de recursos escasos ("Tiempo de palabra") y mecánicas de sigilo/huida.

### 3. Documentos de Diseño (GDD & Referencias)
*Información extraída de la presentación de diseño unificado.*
* **Estética:** Fotorrealismo oscuro inspirado en *Resident Evil 2 Remake* y *Misery Mansion*.
* **Diseño de Nivel:** Estructura laberíntica de la Moncloa y resolución de puzzles ("mini-debates") en escaleras bloqueadas.
* **Arquitectura Técnica:** Diagrama de clases, *Blueprints* de Unreal (GameMode, PlayerController, etc.).

---

## Resumen de Arquitectura del Juego

El juego se estructura sobre la base de clases de Unreal Engine detalladas en el diseño técnico:

| Componente | Descripción |
| :--- | :--- |
| **PedroSanchez_Character** | Protagonista. Gestiona movimiento y "Nivel de Corrupción". |
| **Politicos_Pawn** | Enemigos y aliados reclutables con atributos (Vida, Ataque, Tipo). |
| **GestionMenu_Controller** | Controla la interfaz de inventario y gestión de equipo. |
| **GameModes** | Divididos en `Batalla_GameMode` (combate por turnos) y `MovimientoLibre` (exploración). |

---

## Equipo de Desarrollo (Grupo Pantumaca)

* **Diseño:** Aitor Gómez Ogueta
* **Arte:** Diego Martínez Chamorro
* **Marketing:** Ignacio Hoyos Diego
* **Gestión:** David Covián Gómez
* **Programación:** Javier Yáñez Luzón

---

> *Documento confidencial. Destruir después de leer (o antes de que llegue la Moción de Censura).*
