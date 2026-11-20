# Becify — Plataforma Móvil Centralizada de Becas y Oportunidades Académicas

**Becify** es una aplicación móvil multiplataforma (**Android & iOS**) diseñada para centralizar oportunidades de estudio —**secundaria, grado, posgrado, maestría y doctorado**— conectando a estudiantes con instituciones verificadas bajo un enfoque de **Seguridad desde el Diseño (*Security by Design*)**.

---

## Propósito del Proyecto

Las convocatorias de becas y programas académicos suelen encontrarse dispersas en múltiples portales, dificultando su descubrimiento oportuno y exponiendo a los estudiantes a información desactualizada o enlaces no verificados.

**Becify** resuelve dicha fragmentación mediante una plataforma nativa construida con **Flutter** y **Supabase (PostgreSQL)**, ejecutada bajo el marco ágil **Scrum** y estándares de seguridad **OWASP MASVS**.

---

## Equipo de Ingeniería

| Integrante | Especialidad | Rol en el Proyecto |
| :--- | :--- | :--- |
| **Diana Estephan Ferreras Feliz** | Ingeniería de Software (INTEC) | **Scrum Master**, Líder de Frontend Móvil (**Flutter / Dart**) & Diseño **UI/UX (Figma)** |
| **Deurys Mercedes Batista** | Ciberseguridad | **Líder de Ciberseguridad**, Análisis Forense, Base de Datos Relacional (**PostgreSQL**) & Backend (**Supabase / RLS**) |

---

## Stack Tecnológico Principal

- **Cliente Móvil:** Flutter & Dart (Android / iOS)
- **Base de Datos Relacional:** PostgreSQL (en Supabase) con políticas *Row Level Security (RLS)*
- **Backend & Autenticación:** Supabase Auth, PostgREST API, Storage & Realtime
- **Notificaciones Push:** Firebase Cloud Messaging (FCM)
- **Diseño UI/UX:** Figma
- **Gestión Ágil y Control de Calidad:** GitHub Projects, Issues, Pull Requests protegidos, Dependabot & Secret Scanning

---

## Índice de Documentación Oficial (`/docs`)

Toda la especificación funcional, arquitectónica, de seguridad y de gobernanza ágil se encuentra documentada en el directorio [`/docs`](./docs):

1. [**01 — Visión y Alcance del Producto (PRD)**](./docs/01-vision-y-alcance.md)  
   *Problema, propuesta de valor, perfiles de usuario (`student`, `institution`, `admin`), diagrama de flujo, alcance del MVP vs. Fase 2 y matriz de riesgos.*
2. [**02 — Arquitectura Técnica, Stack y Estrategia de Seguridad**](./docs/02-stack-y-seguridad.md)  
   *Diagrama de arquitectura, justificación técnica (ADRs: Flutter vs. PWA, Supabase PostgreSQL vs. NoSQL), motor de notificaciones, controles de ciberseguridad (RLS, verificación institucional, OWASP MASVS) y requerimientos no funcionales.*
3. [**03 — Gobernanza del Equipo, Marco Scrum y Flujo en GitHub**](./docs/03-equipo-scrum-y-github.md)  
   *Roles del equipo, matriz RACI, ceremonias Scrum adaptadas, hoja de ruta de Sprints (Sprint 0 a Sprint 4), estrategia de ramas, Conventional Commits, Definition of Ready (DoR) y Definition of Done (DoD).*

---

## Estructura del Repositorio

```text
beca-app/
├── .github/                # Configuraciones de flujo de trabajo y plantillas de GitHub
├── app/                    # Código fuente de la aplicación móvil (Flutter / Dart)
├── database/               # Esquemas SQL, migraciones PostgreSQL, políticas RLS y seed data
├── docs/                   # Documentación formal del proyecto
│   ├── 01-vision-y-alcance.md
│   ├── 02-stack-y-seguridad.md
│   ├── 03-equipo-scrum-y-github.md
│   ├── seguridad/          # Modelo de amenazas y auditorías de seguridad
│   └── sprint-0/           # Entregables y actas del Sprint 0
└── README.md               # Portada e índice general del repositorio
```
