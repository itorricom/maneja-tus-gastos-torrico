💰 Maneja tus Gastos

Aplicación Full Stack para gestionar gastos personales.
Permite crear, listar, editar y eliminar gastos mediante una API REST y una interfaz web moderna.

El proyecto está construido con una arquitectura Frontend + Backend + Base de Datos y desplegado en la nube.

🚀 Demo en Producción

🌐 Frontend:
https://maneja-tus-gastos-torrico.web.app

⚙️ Backend API:
https://maneja-tus-gastos-torrico.onrender.com/api/expenses

🧠 Arquitectura
Usuario
   ↓
Frontend (Angular)
   ↓ HTTP API
Backend (Node.js + Express)
   ↓
PostgreSQL
📁 Estructura del Proyecto
maneja-tus-gastos/
│
├── frontend/                # Aplicación Angular
│   ├── src/
│   │   ├── app/
│   │   │   ├── components/
│   │   │   ├── models/
│   │   │   └── services/
│   │   └── environments/
│   │
│   ├── firebase.json
│   └── angular.json
│
├── backend/                 # API Node.js + Express
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   └── db/
│   │
│   └── tests/
│
├── docker-compose.yml
└── README.md
🛠️ Tecnologías Utilizadas

Frontend

Angular

TypeScript

HTML / CSS

Backend

Node.js

Express

Sequelize ORM

Base de Datos

PostgreSQL

DevOps

Docker

Firebase Hosting

Render

GitHub Actions

⚙️ Ejecutar el Proyecto Localmente
1️⃣ Clonar repositorio
git clone https://github.com/TU_USUARIO/maneja-tus-gastos.git
cd maneja-tus-gastos
2️⃣ Configurar variables de entorno
cp backend/.env.example backend/.env
3️⃣ Levantar servicios con Docker
docker-compose up --build
🌐 Servicios Locales
Servicio	URL
Frontend	http://localhost:4200
Backend	http://localhost:3000
Health Check	http://localhost:3000/health
Detener contenedores
docker-compose down

Eliminar también la base de datos:

docker-compose down -v
🧪 Tests
Backend
cd backend
npm install
npm test

Tests implementados con Jest + Supertest.

Frontend
cd frontend
npm install
npm test

Tests con Karma + Jasmine.

📡 API REST
Endpoints
Método	Endpoint	Descripción
GET	/api/expenses	Listar gastos
GET	/api/expenses/	Obtener gasto
POST	/api/expenses	Crear gasto
PUT	/api/expenses/	Actualizar gasto
DELETE	/api/expenses/	Eliminar gasto
Ejemplo de Request
{
  "description": "Supermercado",
  "amount": 50.00,
  "category": "Alimentación",
  "date": "2026-03-08"
}
☁️ Deploy

El proyecto está desplegado usando:

Frontend

Firebase Hosting

Backend

Render

Base de datos

PostgreSQL en Render

⚠️ Nota sobre Render (Plan Free)

El backend puede entrar en reposo tras 15 minutos sin actividad.
La primera petición puede tardar aproximadamente 20-30 segundos.

📌 Mejoras Futuras

Autenticación con JWT

Dashboard con gráficos de gastos

Filtros por categoría

Exportar gastos a Excel / PDF

Progressive Web App (PWA)

👨‍💻 Autor

Isidoro Torrico

Proyecto desarrollado como práctica de arquitectura Full Stack moderna con CI/CD y contenedores.