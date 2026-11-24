# UpTask

Repositorio principal de **UpTask**, una aplicación full stack (MERN + TypeScript) para gestionar proyectos y tareas en equipo. Junta el backend y el frontend como submódulos de Git.

| Submódulo | Descripción |
| --------- | ----------- |
| [`UpTask-Server`](https://github.com/georgemontero1211-spec/UpTask-Server) | API REST con Express, TypeScript, MongoDB/Mongoose, JWT y Nodemailer |
| [`UpTask-Frontend`](https://github.com/georgemontero1211-spec/UpTask-Frontend) | Frontend con React, TypeScript, TanStack Query, React Hook Form y Tailwind CSS |

## Qué hace la aplicación

- Registro de usuarios con confirmación de cuenta por email y recuperación de contraseña.
- Proyectos con un manager y un equipo de colaboradores.
- Tareas con estados: pendiente, en espera, en progreso, en revisión y completada.
- Notas en cada tarea.
- Permisos según el rol del usuario en el proyecto.

## Clonar el proyecto

```bash
git clone --recurse-submodules https://github.com/georgemontero1211-spec/UpTask-Main.git
```

Si ya lo clonaste sin los submódulos:

```bash
git submodule update --init --recursive
```

## Cómo ejecutarlo

1. **Backend**: entra en `UpTask-Server`, crea el `.env` (`DATABASE_URL`, `FRONTEND_URL`, `JWT_SECRET`, `TOKEN_NODEMAILER`) y ejecuta `npm install && npm run dev`.
2. **Frontend**: entra en `UpTask-Frontend`, crea el `.env` con `VITE_API_URL` apuntando a la API y ejecuta `npm install && npm run dev`.

El README de cada submódulo tiene los detalles.
