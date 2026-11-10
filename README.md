# Vínculo — Social Impact & Nonprofit Management

**Public portfolio · Full-stack web prototype · Social impact technology**

[**Ver demostración de Vínculo**](https://vinculo-donantes-1.onrender.com/) · [Estudio de caso](docs/CASE_STUDY.md) · [Arquitectura](docs/ARCHITECTURE.md) · [Guía de entrevista](docs/INTERVIEW.md)

> **Código fuente privado.** Este repositorio es únicamente el portafolio público del proyecto. No incluye frontend, backend, migraciones, credenciales ni datos privados de la aplicación.

## ¿Qué es Vínculo?

Vínculo es un **prototipo en desarrollo** para explorar cómo conectar organizaciones sociales y donantes, y dar seguimiento administrativo a aportaciones. Busca integrar un directorio de organizaciones, cuentas, membresías, registro de donantes y donativos, y una experiencia de demostración para explorar funcionalidades.

**Estado actual:** demostración y pruebas con datos ficticios. **No procesa pagos, no cobra tarjetas y no está preparado para operar con datos reales de donantes.** No debe confundirse un registro manual de donativo con un pago procesado.

## Funcionalidades documentadas

| Módulo | Estado documentado |
|---|---|
| Directorio público | Demostración de tres fundaciones ficticias, filtros y detalles de proyectos |
| Cuentas | Registro, inicio de sesión, consulta y cierre de sesión mediante API |
| Membresías | Consulta de organizaciones asociadas a una cuenta |
| Donantes y donativos | Registro, consulta y edición sujetos a permisos en la API; movimientos manuales, sin cobros |
| Panel de ejemplo | Datos ficticios; parte de la interacción se guarda solo en el navegador |
| Seguimientos de ejemplo | Demostración local, no un seguimiento multiusuario compartido |
| Pagos, verificación de correo y reportes verificados | Pendientes de desarrollo y validación |

Una cuenta nueva no recibe automáticamente acceso administrativo a ninguna fundación.

## Tecnologías del prototipo

- **Frontend:** React, TypeScript, Vite
- **API:** Python, FastAPI, Pydantic
- **Persistencia:** PostgreSQL, migraciones SQL
- **Autenticación:** sesiones, control de membresías, hash de contraseñas
- **Despliegue:** Render (sitio estático, API y base de datos)
- **Ingeniería:** control de versiones, validaciones y documentación técnica

## Flujo conceptual

```text
Organizaciones y campañas → Directorio público
Cuenta de usuario → Autenticación → Membresías y permisos
Gestión administrativa → API → PostgreSQL
Vista de ejemplo → Datos ficticios en la interfaz
```

## Demostración pública

**[Abrir Vínculo en Render](https://vinculo-donantes-1.onrender.com/)**

Para explorar, utiliza **Ver panel de ejemplo** y solo datos ficticios. El servicio gratuito podría tardar en responder tras estar inactivo. Su disponibilidad no está garantizada por este portafolio.

## Qué demuestra este proyecto

- Diseño de una solución tecnológica aplicada a retos de organizaciones sociales.
- Integración de interfaz web, API y base de datos relacional.
- Modelado de cuentas, roles y membresías para gestionar acceso.
- Distinción entre información de demostración y registros persistentes.
- Criterio para definir limitaciones, validaciones y próximas etapas.

## Alcance y precauciones

Vínculo es un **MVP/prototipo**, no una plataforma certificada ni un sistema de procesamiento financiero en operación. Se deben probar los permisos y flujos de extremo a extremo antes de utilizarlo con organizaciones reales. No compartas datos reales de donantes ni credenciales de uso habitual.

## Documentación

- [Estudio de caso y estado de módulos](docs/CASE_STUDY.md)
- [Arquitectura conceptual y privacidad](docs/ARCHITECTURE.md)
- [Cómo explicar Vínculo en una entrevista](docs/INTERVIEW.md)
- [Página visual](index.html)

**Proyecto de portafolio de Fernanda Treviño.** El código de la aplicación está en un repositorio privado distinto.
