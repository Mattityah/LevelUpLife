# LevelUp Life

> Tu progreso, visible. Sincronizado en todos tus dispositivos.

**LevelUp Life** es una app de desarrollo personal gamificada donde cada acción real de tu vida suma experiencia, sube de nivel a tu personaje y construye una identidad visible. Pensada para quien quiere generar estructura, ejecutar ideas y materializar lo que tiene en la cabeza — sin abrumarse.

---

## ¿Qué es?

La vida real tiene un problema de feedback: el progreso es invisible, los loops son largos y no hay recompensa inmediata. LevelUp Life resuelve eso aplicando mecánicas de videojuego (XP, niveles, rachas, nodos neurales) a hábitos y tareas reales.

No es una app de productividad más. Es un espejo de quién estás eligiendo ser cada día.

---

## Features

### Mobile
- **Stack de cartas** — al abrir la app te recibe una carta grande con tu categoría favorita. Swipe arriba para pasar, abajo para volver. Sin menús, sin fricción.
- **Saludo contextual** — buenos días / tardes / noches / ¿trasnochando? con tu nombre y la frase del día
- **Racha visible** — contador de días seguidos en el header, siempre presente
- **Acceso rápido al calendario** — banner entre las cartas y el navbar
- **Cartas personalizables** — podés ocultar y restaurar cartas del stack a gusto

### Desktop
- **Layout de dos columnas** — categorías a la izquierda, panel de progreso a la derecha
- **Panel derecho** — racha con iconos de fuego, anillo de nivel XP, quote motivacional del día, mini calendario
- **Sidebar completo** — navegación, perfil con mini XP bar, notas rápidas, exportar/importar

### Core (mobile + desktop)
- **5 categorías** — Mente, Cuerpo, Skills, Relaciones, Trabajo (personalizables)
- **Sistema de XP y niveles** — cada tarea completada suma puntos, cada nivel tiene un título
- **Red neuronal** — visualización D3.js de tus tareas como nodos que evolucionan (pending → forming → active → myelinated)
- **Habit Tracker** — hábitos con frecuencia diaria, días específicos o X veces por semana. Strip semanal, grilla de 14 días, racha por hábito
- **Bitácora** — notas rápidas con timestamp, organizadas por día, con opción de archivar y exportar
- **Calendario** — vista mensual con actividad diaria y notas por día
- **Firebase Sync** — todos los datos sincronizados en tiempo real entre dispositivos vía Firestore
- **Google Auth** — login con una cuenta de Google, sin contraseñas
- **PWA** — instalable en iOS y Android como app nativa

---

## Stack técnico

| Capa | Tecnología |
|------|-----------|
| Frontend | HTML + CSS + Vanilla JS |
| Visualización | D3.js (force simulation + Canvas) |
| Auth | Firebase Auth (Google Sign-In) |
| Base de datos | Firebase Firestore (realtime sync) |
| Fuentes | Geist 300/400/500 + Instrument Serif |
| Hosting | GitHub Pages |

Sin frameworks. Sin build steps. Un solo archivo `index.html`.

---

## Uso

**App en vivo:** [mattityah.github.io/LevelUpLife](https://mattityah.github.io/LevelUpLife)

1. Abrí el link
2. Iniciá sesión con Google
3. Creá tus primeras tareas en las categorías que te importan
4. Completalas. Mirá cómo sube tu personaje.

---

## Arquitectura de datos

```
state {
  tasks[]         — tareas con categoría, XP, recurrencia
  habits[]        — hábitos con frecuencia y log de días
  activity[]      — log de actividad (max 200 items)
  notes{}         — bitácora por fecha { 'YYYY-MM-DD': 'texto' }
  allCategories[] — categorías activas + custom
  streak          — racha actual en días
  profile{}       — nombre, emoji, gradiente, foto
}
```

Todo se persiste en `localStorage` como fallback y se sincroniza con Firestore cuando hay sesión activa.

---

## Roadmap

### Phase 2 — Backend (DonWeb, PHP + MySQL)
- [ ] Comunidad / feed social (proceso > resultados)
- [ ] Google Calendar write (requiere token management en servidor)
- [ ] Notificaciones push

### Phase 3 — Escala
- [ ] App móvil nativa (iOS / Android)
- [ ] Integración con apps externas (fitness, meditación, idiomas)
- [ ] Sugerencias con IA según historial de actividad

---

## Filosofía de producto

> "Real life has poor feedback architecture — progress is invisible, loops are long. LevelUp Life's core job is making that progress visible and meaningful."

El usuario que entra a esta app no necesita motivación desde cero. Ya quiere cambiar. Necesita una herramienta que acompañe ese proceso haciéndolo visible, disfrutable y sostenible.

**El diferencial:** ningún competidor combina identidad de personaje + desarrollo integral de vida + comunidad enfocada en proceso. Habitica gamifica, pero no construye identidad. Skool conecta, pero no es personal. LevelUp Life hace las tres.

---

## Autor

Construido por **Mattia** — desde cero, con propósito.

*2025*
