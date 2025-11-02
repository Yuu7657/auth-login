# AuthLogin

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.2.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

# 🔐 Auth Login (Angular Session Manager)

Aplicación desarrollada con **Angular** para la **gestión de autenticación, sesiones y protección de rutas**, ideal como módulo base para sistemas con inicio de sesión seguro.  
Incluye manejo de tokens, guardas de navegación (AuthGuard), servicios reutilizables y almacenamiento local para mantener la sesión activa.

---

## 🚀 Descripción general

Este proyecto demuestra un flujo completo de **autenticación de usuarios** en Angular:
- Login con validación reactiva.
- Protección de rutas mediante guardas (`AuthGuard`).
- Mantenimiento de sesión con `LocalStorage` o `SessionStorage`.
- Interceptores para el envío automático de tokens JWT.
- Logout y redirección controlada.

El objetivo es ofrecer una **arquitectura reutilizable** y escalable para cualquier aplicación Angular que requiera autenticación.

---

## 🧩 Características principales

- 🧠 **Login reactivo** con validación por formulario.
- 🔑 **Tokens JWT o simulados** para autenticación.
- 🚷 **Protección de rutas** con `AuthGuard`.
- 💾 **Persistencia de sesión** (LocalStorage / SessionStorage).
- ⚙️ **Interceptor HTTP** para adjuntar tokens a las peticiones.
- 📱 **Diseño adaptable** con Angular Material o CSS puro.

---

## 🧰 Tecnologías utilizadas

| Tecnología | Descripción |
|-------------|-------------|
| **Framework:** | Angular |
| **Lenguaje:** | TypeScript |
| **UI Framework:** | Angular Material |
| **Routing:** | Angular Router |
| **Formularios:** | Reactive Forms |
| **Autenticación:** | JWT (o almacenamiento local simulado) |

---

## 📦 Instalación y ejecución

Clona el repositorio y ejecuta los siguientes comandos:

```bash
git clone https://github.com/Yuu7657/auth-login.git
cd auth-login
npm install
ng serve
auth-login/
│
├── src/
│   ├── app/
│   │   ├── components/      → Componentes de UI (login, dashboard, etc.)
│   │   ├── guards/          → AuthGuard y otras protecciones
│   │   ├── interceptors/    → TokenInterceptor (si aplica)
│   │   ├── services/        → Servicios de autenticación y sesión
│   │   ├── models/          → Interfaces de usuario y token
│   │   ├── app-routing.module.ts
│   │   └── app.module.ts
│   ├── assets/
│   ├── environments/
│   └── index.html
│
├── package.json
├── angular.json
├── tsconfig.json
└── README.md

🔐 Flujo de autenticación

LoginComponent envía las credenciales al AuthService.

El servicio valida o simula la autenticación y guarda el token.

AuthGuard protege las rutas privadas comprobando el token.

Si el token expira o se elimina → redirección automática a /login.

🧭 Próximas mejoras (Roadmap)

🔄 Integración con API real (login y refresh token).

🧱 Sistema de roles y permisos.

💬 Notificaciones de sesión expirada.

📱 Diseño responsive con Angular Material 17.

👨‍💻 Autor

Ricardo Mejía Santillán
Ingeniero en Desarrollo y Gestión de Software
📍 UTOM — Universidad Tecnológica del Oriente de Michoacán
💼 GitHub

🧾 Licencia

Este proyecto se distribuye bajo la licencia MIT.
Eres libre de usarlo, modificarlo y adaptarlo con atribución correspondiente.
