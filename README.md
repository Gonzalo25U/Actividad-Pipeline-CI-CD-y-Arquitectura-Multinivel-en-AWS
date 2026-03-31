# Actividad-Pipeline-CI-CD-y-Arquitectura-Multinivel-en-AWS
 Estructura de Ramas (Contexto de Git Flow)Es vital que cualquier persona que clone tu repo sepa para qué sirven esas tres ramas que mencionas. Puedes añadir una sección de "Desarrollo" así:Markdown## 🛠️ Flujo de Trabajo (Git Flow)

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