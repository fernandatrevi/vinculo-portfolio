# Guía de entrevista | Vínculo

## Pitch de 45 segundos (español)

Vínculo es un prototipo web que desarrollé para explorar cómo conectar organizaciones sociales y donantes con procesos administrativos de seguimiento. Integra una interfaz en React y TypeScript, una API en FastAPI y una base PostgreSQL. El trabajo incluye cuentas, membresías, permisos y registros manuales de donantes y donativos. También diseñé un directorio y un panel de ejemplo para mostrar el concepto. Actualmente utiliza datos ficticios y **no procesa pagos**. Lo presento como experiencia de desarrollo full-stack y modelado de procesos, no como una plataforma financiera lista para producción.

## 45-second pitch (English)

Vínculo is a full-stack prototype designed to explore nonprofit and donor-management workflows. It combines a React and TypeScript interface, a FastAPI backend and PostgreSQL. The project includes user accounts, organization memberships, permissions and manual donor and donation records. It also features a public directory and a sample dashboard. It currently uses fictional data and does not process payments. I present it as an engineering prototype rather than a production-ready financial platform.

## Preguntas y respuestas

**¿Qué problema resuelve?** Explora la integración de información de organizaciones, campañas, donantes y seguimiento, con roles administrativos diferenciados. Todavía no se ha medido un impacto real.

**¿Qué parte funciona?** Según el README privado, existe un directorio ficticio, registro e inicio de sesión por API y persistencia de ciertos datos administrativos. El panel de ejemplo tiene funciones locales que no representan un sistema compartido.

**¿Cómo se almacenan los datos?** PostgreSQL almacena cuentas, membresías y registros de la API; algunos formularios de demostración utilizan almacenamiento del navegador.

**¿Acepta donaciones?** No. Los donativos son registros manuales y no hay integración de cobro.

**¿Qué mejorarías?** Seguridad y privacidad para uso real, suite automatizada de pruebas, validación de permisos en el despliegue, correos, conciliación y métricas de impacto.

**¿Cómo se relaciona con Data Analytics?** Requiere definir entidades, mantener consistencia de registros y diseñar indicadores para analizar campañas y seguimiento. No es evidencia por sí sola de dominio de Snowflake, Power BI o Revenue Management.

**¿Por qué no está el código?** El repositorio original es privado. Esta documentación explica las decisiones técnicas y ofrece una demostración sin distribuir el repositorio.
