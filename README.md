# Actividad-Pipeline-CI-CD-y-Arquitectura-Multinivel-en-AWS
Para mantener la integridad del código y facilitar la entrega continua, este proyecto sigue una estructura de ramificación basada en Git Flow. Es fundamental respetar el propósito de cada rama:

main: Es la rama de producción. Contiene el código estable, probado y listo para el usuario final. Cada cambio aquí genera una nueva versión oficial del sistema.

develop: Es la rama de integración. Aquí es donde se reúnen todas las funcionalidades terminadas antes de pasar a producción. Es el entorno de "pre-estreno" donde se realizan las pruebas de integración.

feature/[nombre-tarea]: Son ramas temporales de desarrollo. Cada vez que vayas a trabajar en una nueva funcionalidad o corrección, debes crear una rama desde develop. Una vez terminada la tarea, se solicita un Pull Request para reintegrarla.

## Este proyecto utiliza una metodología basada en **Git Flow**. Actualmente, el desarrollo se divide en las siguientes ramas de características:

* `feature/frontend`: Desarrollo de la interfaz de usuario y componentes visuales.
* `feature/docker`: Configuración de contenedores, Dockerfiles y orquestación con Docker Compose.
* `feature/docs`: Mejora de la documentación técnica y manuales de usuario.

### Estado del Proyecto
Como estás trabajando en Docker y Frontend por separado, sería genial incluir una pequeña tabla de progreso:

| Módulo | Rama | Estado |
| :--- | :--- | :--- |
| **Frontend** | `feature/frontend` | 🏗️ En desarrollo |
| **Infraestructura** | `feature/docker` | 🐋 Configurando contenedores |
| **Documentación** | `feature/docs` | ✍️ Actualizando README |



### Opción A: Con Docker (Recomendado)
Si estás en la rama `feature/docker`, puedes levantar el entorno con:
\`\`\`bash
docker-compose up --build
\`\`\`

### Opción B: Desarrollo Local (Frontend)
Si prefieres correrlo sin contenedores:
1. Cambia a la rama: \`git checkout feature/frontend\`
2. Instala dependencias: \`npm install\`
3. Corre el proyecto: \`npm run dev\`
4. Visualización del FlujoPara que sea más profesional, puedes incluir un diagrama que explique cómo se mueven tus ramas actuales hacia la meta final.