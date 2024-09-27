# 💇‍♀️ Peluquería The Best - Backend 💻

![Node.js](https://img.shields.io/badge/Node.js-14.17.0-green) ![Express.js](https://img.shields.io/badge/Express.js-4.17.1-blue) ![Sequelize](https://img.shields.io/badge/Sequelize-6.3.5-orange) ![Socket.IO](https://img.shields.io/badge/Socket.IO-%5E4.1.3-lightgrey) ![MySQL](https://img.shields.io/badge/MySQL-8.0.23-yellow)

Este es el repositorio del **Backend** para la plataforma de gestión y e-commerce de una Peluquería/Salón de Belleza. Desarrollado con **Node.js**, **Express**, y **Sequelize**, este backend se encarga de la lógica del servidor, la autenticación, la gestión de la base de datos y las comunicaciones en tiempo real mediante WebSockets.

## 🚀 **Características Principales**

- 🛒 **Gestión de Órdenes**: Soporte completo para la creación de órdenes de compra con productos, métodos de pago y envío.
- 🕒 **WebSockets en Tiempo Real**: Notificaciones en tiempo real para actualizaciones en las reservas y órdenes de compra.
- 📊 **Gráficos de Rendimiento**: Datos de órdenes accesibles para administradores, con gráficos interactivos que muestran el progreso de las ventas.
- 👥 **Gestión de Usuarios y Empleados**: Roles de usuario y asignación de empleados a servicios específicos.
- 🔐 **Autenticación Segura**: Autenticación con **JWT** y protección de rutas.

## 🛠️ **Tecnologías Utilizadas**

- **Node.js**
- **Express.js**
- **Sequelize** (ORM para MySQL)
- **MySQL**
- **Socket.IO**
- **JWT** (JSON Web Tokens) para autenticación
- **Helmet** y **express-rate-limit** para seguridad

## 📦 **Instalación y Ejecución**

1. Clona este repositorio:
   ```bash
   git clone https://github.com/sofia1550/backendIAEcommerce.git
   ```

2. Instala las dependencias:
   ```bash
   cd backendIAEcommerce
   npm install
   ```

3. Crea un archivo `.env` con las siguientes variables:
   ```bash
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=yourpassword
   DB_NAME=peluqueria
   JWT_SECRET=your_jwt_secret
   ```

4. Ejecuta las migraciones y seeders:
   ```bash
   npx sequelize db:migrate
   npx sequelize db:seed:all
   ```

5. Inicia el servidor:
   ```bash
   npm run dev
   ```

6. El servidor estará corriendo en `http://localhost:3001`.

## 📂 **Estructura del Proyecto**

```bash
├── controllers     # Lógica de controladores para las rutas
├── db              # Configuración de la base de datos y modelos
├── middlewares     # Middlewares personalizados (autenticación, etc.)
├── routes          # Definición de rutas del API
├── sockets         # Lógica de WebSockets con Socket.IO
└── utils           # Utilidades y helpers
```

## 🌐 **Enlaces**

- **Frontend**: [Repositorio del Frontend](https://github.com/sofia1550/PeluqueriaTheBest)

## 🛡️ **Seguridad**

- **Autenticación JWT** para la seguridad de los usuarios y protección de rutas.
- **Helmet** y **express-rate-limit** para mitigar ataques comunes como XSS y DDoS.

## 🤝 **Contribuciones**

¡Contribuciones y sugerencias son bienvenidas! No dudes en crear un PR o reportar un issue.

---

Desarrollado con ❤️ por [Nicolás Luciuk](https://www.linkedin.com/in/nicolas-luciuk/)
