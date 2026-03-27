------------------------------------------------EduTrack------------------------------------------------------- 
es una solución integral diseñada para optimizar la labor docente y administrativa en instituciones educativas.
El sistema centraliza la creación de rúbricas, la gestión de notas y el seguimiento del progreso estudiantil, 
eliminando la fragmentación de datos y el trabajo manual repetitivo.

Problema
Los educadores invierten un tiempo excesivo en tareas administrativas manuales, 
lo que reduce la calidad del seguimiento pedagógico individualizado y aumenta el 
riesgo de errores en la consolidación de notas.

Stakeholders
Docentes: Usuarios principales encargados de la evaluación y diseño curricular.
Administradores: Supervisan el cumplimiento de los estándares educativos institucionales.
Estudiantes: Consultan su desempeño para fomentar el aprendizaje autónomo.

Alcance (Scope)
Módulo de creación de rúbricas dinámicas (niveles de desempeño y criterios).
Dashboard de visualización de promedios ponderados por alumno y curso.
Generación automática de reportes trimestrales en formato PDF.

ARQUITECTURA DEL SISTEMA
El sistema utiliza una arquitectura de microservicios para garantizar la escalabilidad y la 
fácil integración de nuevas funcionalidades en el futuro.
    graph TD
    User((Usuario)) --> UI[Frontend - React]
    UI --> GW[API Gateway - FastAPI]
    GW --> S1[Servicio de Rúbricas]
    GW --> S2[Servicio de Calificaciones]
    GW --> S3[Servicio de Usuarios]
    S1 --> DB[(PostgreSQL)]
    S2 --> DB
    S3 --> DB
    S2 --> PDF[Generador de Reportes PDF]







