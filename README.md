🎬 Proyecto de Análisis de Datos SQL: Videoclub
1. Descripción del Proyecto
Este proyecto consiste en un análisis exhaustivo de una base de datos relacional correspondiente a un negocio de alquiler de películas (basada en el esquema Sakila). El objetivo principal es resolver 64 preguntas de negocio que abarcan desde consultas básicas hasta lógica compleja de bases de datos.

A través de este ejercicio, se busca extraer insights sobre el comportamiento de los clientes, la gestión del inventario, la actividad de los actores y el rendimiento financiero de la empresa, utilizando SQL avanzado como herramienta principal.

Técnicas y conceptos aplicados:

Consultas DML: SELECT, INSERT, UPDATE.

Filtrado y Ordenamiento: WHERE, HAVING, ORDER BY.

Agregaciones: COUNT, SUM, AVG, MIN, MAX, STDDEV, VARIANCE.

Joins: INNER JOIN, LEFT JOIN, CROSS JOIN (y análisis de su utilidad).

Subconsultas y CTEs: Lógica anidada para filtros complejos.

Vistas y Tablas Temporales: Creación de estructuras para simplificar análisis recurrentes.

Manejo de Fechas: Cálculos de duración de alquileres y fechas de retorno.

2. Estructura del Proyecto
El proyecto está organizado de la siguiente manera para facilitar su navegación y ejecución:

Plaintext

├── data/
│   └── BBDD_Proyecto.sql       # Script original para la creación y carga de la BBDD
├── queries/
│   └── soluciones_consultas.sql # Archivo con las 64 queries resueltas
└── README.md                   # Documentación del proyecto
3. Instalación y Requisitos
Para reproducir este análisis en tu entorno local, necesitarás:

Motor de Base de Datos: PostgreSQL (recomendado) o cualquier base de datos compatible con SQL estándar (con ligeras modificaciones).

Cliente SQL: DBeaver, pgAdmin, o terminal.

Pasos para ejecutar:

Crea una base de datos vacía.

Ejecuta el script data/BBDD_Proyecto.sql para generar el esquema y poblar los datos.

Abre el archivo queries/soluciones_consultas.sql y ejecuta las consultas según sea necesario.

4. Resultados y Conclusiones
Tras realizar las 64 consultas, se han obtenido conclusiones clave sobre el negocio:

Inventario y Catálogo: Se identificaron películas con características extremas (duración máxima/mínima) y se clasificó el contenido por ratings (ej. PG-13, R), permitiendo entender la distribución demográfica del producto.

Comportamiento del Cliente: Se detectaron los "top clientes" basados en su gasto total y frecuencia de alquiler. También se analizaron patrones de devolución tardía.

Finanzas: Se calculó la variabilidad de los costos de reemplazo (VARIANCE) y los ingresos totales, proporcionando una visión clara de la salud financiera y el riesgo de inventario.

Actores: Se generaron métricas de productividad por actor, identificando a los más activos y cruzando datos con categorías específicas (ej. Actores de 'Action').

5. Próximos Pasos
Para escalar este proyecto y aportar más valor en el futuro, se proponen las siguientes acciones:

Visualización: Conectar la base de datos a una herramienta de BI (como Tableau o PowerBI) para crear dashboards interactivos sobre las ventas mensuales.

Optimización: Analizar el plan de ejecución (EXPLAIN ANALYZE) de las consultas más pesadas (ej. las que usan múltiples JOINs) e implementar índices donde sea necesario.

Automatización: Crear Stored Procedures para reportes mensuales automáticos de ingresos y clientes morosos.

6. Contribuciones
Las contribuciones son bienvenidas. Si tienes una forma más eficiente de realizar alguna de las consultas complejas o encuentras un error, por favor:

Haz un Fork del repositorio.

Crea una nueva rama (git checkout -b feature/nueva-consulta).

Envía un Pull Request.

7. Autores y Agradecimientos
Autor: [Tu Nombre]

Agradecimientos: Al equipo de DataProject por plantear el reto de lógica SQL y proporcionar el dataset de prueba.
