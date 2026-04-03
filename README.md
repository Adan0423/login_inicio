# Sistema de Autenticación - Login Inicial

Un proyecto de interfaz de login con sistema de autenticación desarrollado como proyecto final durante mis estudios. La aplicación proporciona una plataforma segura para el inicio de sesión de usuarios con validación de credenciales.

## 📋 Descripción del Proyecto

Este proyecto es un sistema de autenticación basado en web que permite a los usuarios registrarse e iniciar sesión de manera segura. Fue desarrollado como ejercicio académico para aprender los fundamentos de la seguridad web, validación de formularios y comunicación asincrónica con bases de datos.

## 🛠️ Tecnologías Utilizadas

- **Frontend:**
  - HTML5 - Estructura del documento
  - CSS3 - Estilos y diseño responsivo (con `estilos.css`)
  - JavaScript (Vanilla JS) - Lógica de cliente
  - jQuery 3.3.1 - Manipulación del DOM y peticiones AJAX
  - Bootstrap 4 - Framework CSS para diseño responsive
  - SweetAlert2 - Alertas y notificaciones personalizadas

- **Backend:**
  - PHP - Procesamiento del servidor y lógica de autenticación
  - MySQL 5.6+ - Base de datos para almacenamiento de usuarios

- **Complementos:**
  - Popper.js - Gestor de posicionamiento de elementos
  - Material Design Iconic Font - Iconografía

## 📁 Estructura del Proyecto

```
login_inicio/
├── index.php                 # Página principal de login
├── codigo.js                 # Scripts de validación y AJAX
├── estilos.css              # Estilos personalizados
├── login_2019.sql           # Script de base de datos SQL
│
├── bd/                      # Directorio de base de datos
│   └── login.php            # Procesamiento de autenticación
│
├── vistas/                  # Vistas adicionales
│   └── pag_inicio.php       # Página de inicio post-login
│
├── bootstrap/               # Framework Bootstrap
│   ├── css/
│   └── js/
│
├── jquery/                  # Librería jQuery
├── popper/                  # Librería Popper.js
├── plugins/                 # Plugins adicionales
│   └── sweetalert2/         # Notificaciones SweetAlert2
│
├── fuentes/                 # Fuentes e iconografía
│   └── iconic/
│
└── plugins/                 # Plugins externos

```

## ⚙️ Características Principales

- ✅ **Interfaz de Login Intuitiva** - Diseño limpio y responsivo
- ✅ **Validación de Formularios** - Validación en cliente y servidor
- ✅ **Autenticación de Usuarios** - Sistema de login con usuario y contraseña
- ✅ **Alertas Personalizadas** - Notificaciones SweetAlert2 para feedback del usuario
- ✅ **Solicitudes AJAX** - Comunicación asincrónica sin recargar la página
- ✅ **Almacenamiento Seguro** - Base de datos MySQL para persistencia de datos
- ✅ **Diseño Responsivo** - Adaptable a diferentes dispositivos

## 🚀 Instalación y Configuración

### Requisitos Previos

- PHP 5.5+ (compatible con versiones modernas)
- MySQL 5.6+
- Servidor web (Apache, Nginx, etc.)
- Navegador web moderno

### Pasos de Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/Adan0423/login_inicio.git
   cd login_inicio
   ```

2. **Configurar la base de datos:**
   - Abre tu gestor de base de datos (phpMyAdmin, MySQL Workbench, etc.)
   - Importa el archivo `login_2019.sql`:
     ```sql
     CREATE DATABASE login_2021;
     USE login_2021;
     SOURCE login_2019.sql;
     ```

3. **Configurar la conexión a BD:**
   - Edita el archivo `bd/login.php` con tus credenciales de MySQL:
     ```php
     $host = 'localhost';
     $usuario_bd = 'root';
     $password_bd = '';
     $base_datos = 'login_2021';
     ```

4. **Colocar los archivos en el servidor:**
   - Coloca los archivos en la carpeta web de tu servidor (`htdocs` en XAMPP, `www` en WAMP, etc.)

5. **Acceder a la aplicación:**
   - Abre tu navegador y ve a: `http://localhost/login_inicio/`

## 👤 Credenciales de Prueba

Por defecto, la base de datos incluye dos usuarios de prueba:

| Usuario | Contraseña |
|---------|-----------|
| admin   | 12345     |
| demo    | 123456    |

> ⚠️ **Nota de Seguridad:** Estas credenciales son solo para propósitos de demostración y prueba. Cambiar las contraseñas antes de poner en producción.

## 📝 Uso de la Aplicación

1. Ingresa a `index.php`
2. Completa los campos de **Usuario** y **Password**
3. Haz clic en el botón **CONECTAR**
4. Si las credenciales son correctas, serás redirigido al dashboard
5. Si hay un error, recibirás una notificación SweetAlert2

## 🔒 Consideraciones de Seguridad

- Las contraseñas se almacenan con hash MD5 (considerar actualizar a bcrypt o similar para producción)
- Se valida tanto en cliente como en servidor
- Se utilizan peticiones AJAX para mayor seguridad
- Se trimean los inputs para evitar espacios innecesarios

## 📚 Aprendizajes Clave

Este proyecto demuestra conceptos fundamentales:

- **Validación de formularios** con JavaScript
- **Comunicación AJAX** entre cliente y servidor
- **Autenticación básica** de usuarios
- **Manejo de bases de datos MySQL** con PHP
- **Diseño UI/UX** responsivo y atractivo
- **Integración de librerías externas** (jQuery, Bootstrap, SweetAlert2)

## 🎓 Contexto Académico

Este proyecto fue desarrollado como trabajo final de un curso/módulo de desarrollo web durante mi formación académica. Representa los conocimientos adquiridos en:
- Desarrollo Frontend
- Programación Backend con PHP
- Administración de Bases de Datos
- Buenas prácticas en programación web

## 📄 Licencia

Este proyecto se proporciona con fines educativos.

## 👨‍💻 Autor

**Adan0423** - [GitHub](https://github.com/Adan0423)

---

**Última actualización:** Abril 2026