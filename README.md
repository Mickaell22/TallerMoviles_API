# serverDawa — Backend

API REST para sistema de gestión de taller de reparación de teléfonos. Módulos de reparaciones, repuestos, técnicos, usuarios y órdenes.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

> Proyecto académico — Desarrollo de Aplicaciones Web · Universidad de Guayaquil

---

## Módulos

| Módulo | Rutas |
|--------|-------|
| **Reparaciones** | CRUD por cédula, técnico e ID |
| **Repuestos** | CRUD con filtros por proveedor y categoría |
| **Técnicos** | Gestión de personal técnico con especialidad |
| **Usuarios** | Registro, login, roles |
| **Órdenes** | Órdenes de trabajo con detalle de productos |

---

## Stack

| Capa | Tecnología |
|------|-----------|
| Runtime | Node.js |
| Framework | Express |
| ORM | Prisma (migraciones incluidas) |
| Auth | JWT (`jsonwebtoken`) + bcrypt |
| Base de datos | PostgreSQL / MySQL (configurable en Prisma) |

---

## Correr localmente

```bash
git clone https://github.com/Mickaell22/TallerMoviles_API.git
cd TallerMoviles_API
npm install
```

Configura la conexión en `config/env.js` con tu `DATABASE_URL`, luego:

```bash
npx prisma migrate dev
node server.js
```

---

## Frontend

Consumido por [TallerMoviles_Frontend](https://github.com/Mickaell22/TallerMoviles_Frontend) — React SPA.
