# Documentación del Proyecto Netflix

## Descripción General
Este proyecto es una réplica de la interfaz de Netflix, implementando funcionalidades básicas de streaming de contenido, sistema de usuarios y reproducción de videos.

## Estructura del Proyecto

### Frontend
- `index.html`: Página principal después del inicio de sesión
- `login.html`: Página de inicio de sesión
- `css/`: Directorio de estilos
  - `style.css`: Estilos principales
  - `login.css`: Estilos específicos para el login
- `js/`: Directorio de scripts
  - `main.js`: Funcionalidades principales
  - `login.js`: Manejo del formulario de login
- `img/`: Directorio de imágenes y recursos visuales

### Backend
- `conexion.php`: Conexión a la base de datos
- `comprobar.php`: Validación de inicio de sesión
- `insertar_usuario.php`: Script para agregar usuarios

### Base de Datos
- Nombre: `dbnetflix`
- Tabla: `tclientes`
  - `Email`: Correo electrónico del usuario
  - `password`: Contraseña hasheada

## Funcionalidades Implementadas

### Sistema de Usuarios
1. Registro de usuarios
2. Inicio de sesión
3. Validación de credenciales
4. Manejo de sesiones

### Interfaz de Usuario
1. Diseño responsive
2. Navegación intuitiva
3. Reproductor de video
4. Lista de películas y series

### Seguridad
1. Contraseñas hasheadas
2. Protección contra SQL injection
3. Validación de datos
4. Manejo de sesiones seguras

## Requisitos del Sistema

### Software
- XAMPP (Apache + MySQL + PHP)
- Navegador web moderno
- Editor de código (recomendado: VS Code)

### Hardware
- Procesador: 1.6 GHz o superior
- RAM: 4GB mínimo
- Espacio en disco: 1GB libre

## Instalación

1. Clonar o descargar el repositorio
2. Colocar los archivos en el directorio htdocs de XAMPP
3. Iniciar XAMPP (Apache y MySQL)
4. Crear la base de datos:
   ```sql
   CREATE DATABASE dbnetflix;
   USE dbnetflix;
   CREATE TABLE tclientes (
       Email VARCHAR(255) PRIMARY KEY,
       password VARCHAR(255) NOT NULL
   );
   ```
5. Ejecutar `insertar_usuario.php` para crear usuario de prueba

## Uso del Sistema

### Inicio de Sesión
1. Acceder a `login.html`
2. Ingresar credenciales:
   - Email: aaron@gmail.com
   - Password: 123456
3. Ser redirigido a `index.html` si las credenciales son correctas

### Navegación
1. Menú principal con categorías
2. Búsqueda de contenido
3. Reproducción de videos
4. Perfil de usuario

## Estructura de Archivos
```
proyecto-netflix/
├── index.html
├── login.html
├── conexion.php
├── comprobar.php
├── insertar_usuario.php
├── css/
│   ├── style.css
│   └── login.css
├── js/
│   ├── main.js
│   └── login.js
└── img/
    └── [recursos visuales]
```

## Mantenimiento

### Actualizaciones
1. Verificar compatibilidad de versiones
2. Hacer backup de la base de datos
3. Actualizar archivos
4. Probar funcionalidades

### Backup
1. Base de datos: Exportar regularmente
2. Archivos: Mantener copia de seguridad
3. Configuraciones: Documentar cambios

## Solución de Problemas

### Errores Comunes
1. Error de conexión a base de datos
   - Verificar XAMPP
   - Comprobar credenciales
   - Revisar configuración

2. Problemas de inicio de sesión
   - Verificar credenciales
   - Comprobar sesiones
   - Revisar redirecciones

3. Errores de visualización
   - Limpiar caché del navegador
   - Verificar rutas de archivos
   - Comprobar permisos

## Mejoras Futuras
1. Implementar registro de usuarios
2. Agregar sistema de perfiles
3. Mejorar el reproductor de video
4. Implementar búsqueda avanzada
5. Agregar sistema de recomendaciones

## Contacto y Soporte
Para reportar problemas o sugerir mejoras:
1. Revisar la documentación
2. Verificar errores comunes
3. Contactar al equipo de desarrollo

## Licencia
Este proyecto es para fines educativos y de demostración. 