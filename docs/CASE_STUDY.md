# Vínculo | Estudio de caso

## 1. Problema abordado

Organizaciones sociales pueden enfrentar retos al organizar la información de campañas, donantes y seguimiento. Vínculo explora una plataforma que conecte la experiencia de consulta de proyectos con un espacio administrativo. Esta es la **motivación del diseño**, no un hallazgo medido en organizaciones participantes.

## 2. Propuesta de valor

Ofrecer en una misma experiencia un directorio de fundaciones y funciones administrativas, con membresías y permisos. El objetivo a futuro es vincular aportaciones registradas con procesos de agradecimiento y seguimiento, sujeto a desarrollo y validación.

## 3. Estado funcional actual

| Componente | Estado de la implementación |
|---|---|
| Directorio público | Tres fundaciones ficticias con filtros y fichas de proyectos |
| Registro y acceso | Cuentas, inicio/cierre de sesión y consulta de cuenta mediante API |
| Organizaciones asociadas | Consulta mediante membresías; las cuentas nuevas no tienen acceso automático |
| Datos administrativos | Donantes y donativos manuales: consulta, registro y edición según permisos en PostgreSQL |
| Panel de ejemplo | Datos de demostración y algunas operaciones en localStorage |
| Seguimientos de ejemplo | Simulación local, no sistema colaborativo persistente |
| Pagos en línea | No implementados |
| Verificación de email | Pendiente |
| Suscripciones/notificaciones/reportes verificados | Pendientes |

Los resultados locales de prueba no equivalen a validación integral de la aplicación desplegada.

## 4. Herramientas y capacidades

- React + TypeScript + Vite para experiencia web.
- FastAPI + Pydantic para lógica de la API.
- PostgreSQL + SQL para persistencia y migraciones.
- Autenticación y permisos asociados a membresías.
- Render para publicación de interfaz y API en servicios separados.

## 5. Flujo de usuario ejemplificado

1. Una persona explora el directorio público.
2. Si desea crear cuenta, completa el registro con datos ficticios durante la demostración.
3. Inicia sesión y consulta su cuenta.
4. Si no tiene una membresía asignada, no puede administrar una fundación.
5. Las funciones administrativas están condicionadas por permisos; el panel de ejemplo no representa una operación compartida real.

## 6. Indicadores potenciales (no implementados como resultados comprobados)

En una siguiente etapa podrían medirse aportaciones confirmadas, tasa de recurrencia, tiempo de agradecimiento, retención de donantes y cumplimiento de seguimientos. Para eso serían necesarios datos confiables, definiciones compartidas y reglas de conciliación.

## 7. Limitaciones y próximos pasos

- No utilizar datos reales de donantes hasta completar controles de seguridad y validación.
- Agregar verificación de correo y pruebas automatizadas de flujos críticos.
- Corregir los pendientes de lint y verificar controles de acceso en despliegue.
- Diseñar conciliación contable antes de hablar de donaciones cobradas.
- Definir condiciones de seguridad, privacidad y tratamiento de datos.
- Evaluar métricas con organizaciones piloto solamente después de validación.

## 8. Aprendizajes técnicos

El proyecto permite explicar decisiones de diseño de datos, integración frontend/backend, persistencia, permisos y diferencias entre simulación y operación real.

**Demostración:** https://vinculo-donantes-1.onrender.com/ — puede tardar al iniciar en un plan gratuito.

*Este documento no incluye ni revela código fuente del repositorio privado.*
