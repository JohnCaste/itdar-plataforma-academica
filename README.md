# ITDAR — Plataforma académica 
### Caso de estudio · Desarrollo full-stack con enfoque backend

Plataforma web que digitalizó la gestión académica del Instituto Teológico
David Arcos Ríos (Río Blanco, Veracruz) y que hizo posible abrir su
modalidad virtual.

**Sitio en producción:** [itdar.org](https://itdar.org) · En uso desde 18 de abril de 2023
El código fuente es privado porque maneja datos institucionales.
Puedo mostrarlo y explicarlo en una entrevista.

---

## Contexto
ITDAR es un instituto teológico con dos modalidades: **presencial**
(~50 usuarios entre alumnos y maestros) y **virtual** (13 alumnos).

## El problema
Toda la operación académica dependía de Excel, Word, correo electrónico
y trámites en persona: calificaciones, documentos, tareas y
comunicación alumno-maestro. Además, sin una plataforma no existía forma de ofrecer
una **modalidad virtual**.

## La solución
Una plataforma con portales separados por rol:

| Alumnos | Maestros | Administración |
|---|---|---|
| Materias con recursos, temario y entrega de tareas | Publicación de recursos y revisión de tareas con retroalimentación | Admisión virtual con links de invitación y revisión de solicitudes |
| Kárdex y boleta descargable en PDF | Generación de cuestionarios de práctica con IA a partir de un PDF | Alta y gestión de alumnos y maestros |
| Calendario de clases del cuatrimestre | Gestión de calificaciones | Inventario de activos con etiquetas QR |
| Plan de lectura bíblica con seguimiento de avance | | Anuncios, indicadores y encuestas |
| Notificaciones | | Sincronización de clases virtuales con Google Meet |

## Stack
- **Frontend:** Angular · design system propio · Firebase Hosting
- **Backend:** Python · Flask · gunicorn · Google Cloud Run
- **Datos:** BigQuery, con datasets separados por entorno (DEV/PROD) y modalidad
- **Integraciones:** Gemini API (IA), Google Meet, correo SMTP
- **Prácticas:** registros de decisiones de arquitectura (ADR), especificaciones con OpenSpec

## Mi rol
Desarrollador principal: diseño, arquitectura e implementación de la
plataforma completa, con la mentoría de un desarrollador senior.

<!-- PENDIENTE: Arquitectura · Decisiones técnicas · Retos · Capturas · Lo que aprendí -->
