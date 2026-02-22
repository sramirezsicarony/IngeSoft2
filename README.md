📚 Sistema de Biblioteca – Backend con Spring Boot
📖 Descripción del Proyecto

Este proyecto consiste en el desarrollo de una aplicación backend para la gestión de una biblioteca, implementada con Spring Boot y JPA bajo una arquitectura en capas.

El sistema permite realizar búsquedas inteligentes de libros basadas en porcentaje de similitud, así como gestionar calificaciones y reseñas en tiempo de ejecución. La aplicación está diseñada inicialmente para ejecutarse por consola, permitiendo validar la lógica del negocio antes de implementar una interfaz web.

🏗 Arquitectura

El proyecto sigue una arquitectura en capas:

Domain → Entidades y lógica del negocio.

Repository → Persistencia de datos mediante JPA.

Service → Implementación de casos de uso.

Presentation (Console) → Interacción con el usuario por consola.

Se aplica separación de responsabilidades y principios SOLID para garantizar escalabilidad y mantenibilidad.

⚙ Tecnologías Utilizadas

Java 17+

Spring Boot

Spring Data JPA

Hibernate

Base de datos relacional (MySQL / PostgreSQL)

Maven

🚀 Funcionalidades
🔍 Búsqueda Simple

Permite buscar libros por título o autor, ordenados de mayor a menor según el porcentaje de similitud.

🔎 Búsqueda Combinada

Permite buscar libros utilizando múltiples criterios (título, subtítulo, autor, año y epílogo), calculando una puntuación total de coincidencia.

⭐ Calificación de Libros

Los usuarios pueden calificar libros con una puntuación del 1 al 5. Las calificaciones se almacenan en memoria durante la ejecución del programa.

📝 Reseñas

Permite escribir reseñas para cualquier libro, con confirmación previa antes de ser almacenadas en memoria.

🧠 Características Técnicas Destacadas

Ordenamiento automático de resultados mediante TreeSet y Comparator personalizado.

Cálculo de porcentaje de similitud en capa de servicio.

Persistencia exclusiva de libros en base de datos.

Calificaciones y reseñas gestionadas en memoria.

Diseño preparado para futura migración a API REST.

👥 Equipo de Desarrollo

Proyecto desarrollado bajo metodología Scrum, con distribución de responsabilidades por capas:

Infraestructura y Persistencia

Modelado de Dominio

Servicios de Búsqueda

Gestión de Reseñas y Calificaciones

Interfaz por Consola
