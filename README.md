# Proyecto: Sistema de Gestión de Tareas para Estudiantes (StudyTasks)

## Objetivo
Desarrollar una aplicación web que permita a los estudiantes organizar sus tareas, establecer fechas límite y recibir recordatorios.

---

## Requisitos Funcionales del Proyecto

### Gestión de usuarios
1. El sistema debe permitir a los usuarios registrarse proporcionando:
   - Nombre de usuario.
   - Correo electrónico.
   - Contraseña segura.
2. Los usuarios deben poder iniciar sesión en su cuenta utilizando:
   - Correo electrónico.
   - Contraseña.
3. El sistema debe incluir una opción para recuperar la contraseña en caso de que el usuario la olvide.

### Gestión de tareas (CRUD)
1. Los usuarios deben poder **crear tareas**, proporcionando:
   - Título de la tarea.
   - Descripción de la tarea.
   - Nivel de prioridad (baja, media, alta).
   - Fecha de vencimiento.
2. Los usuarios deben tener acceso a una lista de todas sus tareas:
   - Agrupadas por estado (pendiente o completada).
   - Ordenadas por fecha de vencimiento.
3. El sistema debe permitir **editar** las tareas existentes, incluyendo:
   - Cambios en el título, descripción, prioridad o fecha de vencimiento.
4. Los usuarios deben poder **eliminar** tareas:
   - Tanto completadas como pendientes, según sea necesario.

### Sistema de recordatorios
1. El sistema debe enviar recordatorios a los usuarios cuando:
   - Una tarea esté próxima a su fecha de vencimiento.
2. Los recordatorios pueden implementarse de la siguiente manera:
   - Notificaciones internas dentro de la aplicación.
   - Correos electrónicos enviados al usuario registrado.

### Interfaz amigable
1. La aplicación debe ser intuitiva y fácil de usar, con:
   - Navegación clara entre secciones (registro, inicio de sesión, lista de tareas, etc.).
   - Retroalimentación visual para acciones como la creación, edición y eliminación de tareas.
2. Debe garantizar una experiencia consistente y eficiente para el usuario.

### Seguridad
1. Todas las contraseñas deben estar encriptadas antes de almacenarse en la base de datos.
2. El sistema debe validar y sanitizar todos los datos ingresados por los usuarios, con el fin de prevenir:
   - Ataques como la inyección SQL.
   - Errores comunes en la entrada de datos.

---

### Requisitos técnicos
1. **Frontend**: HTML, CSS, JavaScript. Opcional: Frameworks como React, Angular o Vue.js.
2. **Backend**: Python con Flask/Django, Node.js con Express, o PHP.
3. **Base de datos**: MySQL, PostgreSQL o MongoDB para almacenar usuarios y tareas.
4. **Control de versiones**: Uso de Git para manejar el progreso del proyecto.
5. **Hosting**: Desplegar la aplicación en una plataforma como Heroku o Vercel.

---

## Fases de desarrollo

### Fase 1: Planeación y definición
1. **Especificación de requisitos**: Crear una lista detallada de requisitos y confirmarlos.
2. **Diseño conceptual**:
   - Diseñar mockups para las pantallas principales (registro, inicio de sesión, lista de tareas).
   - Crear diagramas de flujo de datos para entender cómo se moverán los datos entre el usuario y la base de datos.

### Fase 2: Configuración del entorno
3. **Seleccionar tecnologías**: Elegir las herramientas y lenguajes que usarás.
4. **Crear la base del proyecto**:
   - Configurar un repositorio en GitHub o GitLab para registrar avances.
   - Configurar el ambiente de desarrollo con los frameworks, base de datos y servidor local.

### Fase 3: Desarrollo por etapas
5. **Primera funcionalidad: Sistema de usuario**:
   - Implementar el registro e inicio de sesión de usuarios con validación de datos.
6. **Segunda funcionalidad: Gestión de tareas**:
   - Desarrollar funciones CRUD para las tareas.
   - Implementar una interfaz para visualizar y gestionar tareas.
7. **Tercera funcionalidad: Recordatorios automáticos**:
   - Crear el sistema de notificaciones por correo o en la misma aplicación.

### Fase 4: Pruebas y ajuste final
8. **Pruebas unitarias y de integración**:
   - Verificar que cada funcionalidad funcione correctamente y probar la integración completa.
9. **Despliegue**:
   - Subir la aplicación a un servidor como Heroku o Vercel.
10. **Documentación**:
    - Crear una guía para el usuario final y documentación técnica del proyecto.

---

## Estándares para el desarrollo de software

1. **Estándares de codificación**:
   - Utilizar nombres descriptivos para variables, funciones y clases.
   - Seguir la convención de nomenclatura del lenguaje (por ejemplo, camelCase para JavaScript, snake_case para Python).
   - Mantener un código limpio y bien comentado.

2. **Pruebas**:
   - Realizar pruebas unitarias para cada componente individual.
   - Implementar pruebas de integración para verificar el funcionamiento conjunto de los módulos.

3. **Control de versiones**:
   - Realizar commits frecuentes con mensajes claros y descriptivos.
   - Utilizar ramas para diferentes funcionalidades y fusionarlas cuidadosamente.

4. **Seguridad**:
   - Validar y sanitizar datos de entrada para evitar ataques como la inyección SQL.
   - Usar HTTPS y cifrar contraseñas de los usuarios (por ejemplo, con bcrypt).

5. **Documentación**:
   - Mantener documentación actualizada del proyecto, incluyendo dependencias y configuraciones.
   - Crear manuales de usuario y guías técnicas.

6. **Estándares de diseño**:
   - Diseñar una interfaz amigable y accesible.
   - Seguir principios de diseño como consistencia, claridad y retroalimentación al usuario.

---

## Guía para el desarrollo

### Planeación
- Define claramente los requisitos del cliente (en este caso, yo).
- Diseña los mockups y diagramas para visualizar la estructura del sistema.

### Configuración del entorno
1. Instala las herramientas necesarias:
   - Framework elegido (por ejemplo, Flask o React).
   - Base de datos (por ejemplo, MySQL).
   - Sistema de control de versiones (Git).
2. Configura tu ambiente de desarrollo: asegúrate de que tu entorno local esté listo para ejecutar el proyecto.

### Desarrollo
- **Sistema de usuario**: Implementa un modelo de base de datos para los usuarios y las funciones de registro/inicio de sesión.
- **Gestión de tareas**: Diseña el modelo de datos para las tareas y desarrolla las funciones CRUD.
- **Recordatorios**: Usa una librería o servicio como `nodemailer` (para Node.js) o `smtplib` (para Python) para enviar correos electrónicos, si decides usarlos.

### Pruebas y despliegue
- Realiza pruebas unitarias para cada funcionalidad.
- Integra y prueba todo el sistema.
- Despliega la aplicación y verifica su funcionamiento en el servidor.

---

## Evaluación
Como tu cliente, revisaré:
1. Cumplimiento de requisitos.
2. Calidad del código (legibilidad, comentarios).
3. Funcionalidad y experiencia del usuario.
4. Documentación técnica y manual del usuario.

---
