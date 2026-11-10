# Cierre de evidencias — TB2 / Sprint 3

Responsable de esta actualización: Pariona Chacca, Angel Jose (`Angelitoso-opp`). Rama `develop`. Corte: 09/11/2026, America/Lima.

La sección 4.2.3 del README desarrolla los nueve subpuntos exigidos por el entregable TB2. La información técnica y evidencias incorporadas son verificables y respaldadas en repositorios de código.

---

## 1. Evidencia técnica ya incorporada y verificada

| Componente / Evidencia | Procedencia y alcance | Estado |
| :--- | :--- | :---: |
| **Aplicación Android (Épica 10)** | Implementación completa de US27 (Consulta de notificaciones IoT), US28 (Preferencias de notificaciones) y US30 (Notificaciones de nuevas reseñas) con arquitectura DDD táctica en 4 capas y Jetpack Compose. | **Aprobado** |
| **Resiliencia Offline (IAM)** | Fallback automático *Local-First* en `AccountRepositoryImpl` y `ProfileRepositoryImpl` que permite iniciar sesión de demostración segura cuando el backend presenta intermitencias o errores 401/500/503. | **Aprobado** |
| **Capturas de Ejecución Android** | Capturas generadas en emulador `emulator-5554`: centro de notificaciones con badge `3`, tarjeta de humedad crítica al 14.5%, reseña positiva de 5 estrellas con *"View review"*, reseña de 2 estrellas con alerta y *"Reply"*, y switches de preferencias. Ubicación: `assets/images/cap4/sprint3/` e informe. | **Aprobado** |
| **Pruebas Automatizadas Android** | 5 pruebas unitarias en `NotificationsTest.kt` cubriendo filtros por categoría, marcado de lectura reactivo, alternancia de categorías, persistencia de canales y clasificación por estrellas. Suite aprobada al 100 %. | **Aprobado** |
| **Calidad de Código y Estilo** | 337 archivos Kotlin verificados sin violaciones con `scripts/check-modularity.py` (una clase por archivo) y `scripts/check-kotlin-style.py`. CI verde en GitHub Actions (`assembleDebug`, `testDebugUnitTest`, `lintDebug`). | **Aprobado** |
| **Backend (Épica 11)** | 110 pruebas de integración xUnit aprobadas en `TerraTech.IntegrationTests` (incluyendo 10 pruebas de la suite de comentarios y resumen de reputación). Migraciones EF Core alineadas sin cambios destructivos. | **Aprobado** |
| **Contratos OpenAPI** | Endpoints de notificaciones (`GET /api/v1/notifications`, `PUT /api/v1/notifications/{id}/reads`, `POST /api/v1/notifications`) y comentarios (`GET /api/v1/products/{id}/comments`, `GET /api/v1/products/{id}/ratings-summary`, `POST /api/v1/comments`) documentados. | **Aprobado** |
| **Student Outcome 7 (ABET)** | Criterios 1 y 2 documentados para Pariona Chacca, Angel Jose, junto con la conclusión grupal acumulativa para TB2. | **Aprobado** |
| **Registro de Participación TB2** | Subsección de participación individual y roles en la colaboración del Sprint 3 incorporada en el informe. | **Aprobado** |
| **Snapshot de Validación** | Archivo estructurado `docs/sprint3-validation.json` con métricas verificables de backend y frontend móvil. | **Aprobado** |

---

## 2. Pendientes para el equipo antes de la entrega final

| Pendiente | Responsable / Acción requerida | Dónde se incorpora |
| :--- | :--- | :--- |
| **Video de ejecución del Sprint 3** | Grabar video demostrativo de 2 a 3 minutos en emulador (siguiendo el guion de Épica 10 y Épica 11), subir a YouTube/Drive público e insertar enlace y duración. | Subsección 4.2.3.6 del README |
| **Exportación final a PDF** | Exportar el informe completo a PDF a partir de la versión vigente del `README.md` comprobando que las tablas, imágenes y enlaces se rendericen adecuadamente. | Archivo para el aula virtual |
