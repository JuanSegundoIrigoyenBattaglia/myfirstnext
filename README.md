# Consultorio odontologico en Next.js

Migracion de la pagina estatica a Next.js con App Router, Firebase Auth, Firestore y App Check.

## Configuracion

1. Copia `.env.local.example` como `.env.local`.
2. Completa las variables `NEXT_PUBLIC_FIREBASE_*`.
3. Si usas App Check, completa `NEXT_PUBLIC_RECAPTCHA_ENTERPRISE_SITE_KEY`.
4. Instala dependencias con `npm install`.
5. Levanta el proyecto con `npm run dev`.

## Firebase

Usa las mismas colecciones y reglas del proyecto original:

- `turnos`
- `turnosOcupados`
- `userTurnosPendientes`
- `admins`

El documento admin debe usar el UID de Firebase Auth como ID y tener:

```text
activo    boolean    true
```
