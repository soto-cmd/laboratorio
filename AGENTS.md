# Agentes Soto — política del repositorio

Estas instrucciones son para asistentes de código y revisores automáticos. Aplicar las skills en `.agents/skills/` de forma selectiva.

## Reglas obligatorias
- NUNCA desplegar, fusionar PR, modificar producción, ejecutar migraciones, importar o eliminar registros sin autorización expresa.
- Preservar funcionalidades, datos, publicidad, contenido y archivos ya existentes. Nada de refactors masivos.
- Antes de editar: inspeccionar el código actual, registrar comportamiento esperado, dependencias, riesgos y plan de reversión.
- Trabajar exclusivamente en rama aislada; cambios pequeños y PR revisables. Evitar builds repetidos y llamadas innecesarias.
- Respaldar con fecha, versión e identificador antes de cualquier operación riesgosa sobre datos. No afirmar backups sin evidencia.
- Proteger contra XSS, inyección, acceso no autorizado y secretos expuestos. Revisar RLS en Supabase; no desactivar protecciones.
- Sin credenciales reales, cambios en cuentas, ni consultas intensivas a Neon/Supabase/Vercel sin justificación.
- Informes breves en tres grupos: Requiere atención / Preparado, pendiente de integrar o desplegar / Verificado.
- Diferenciar revisión estática, pruebas ejecutadas y pruebas pendientes; no atribuir éxito a verificaciones no efectuadas.

## Skills
- `.agents/skills/seguridad/SKILL.md`
- `.agents/skills/proteccion-datos/SKILL.md`
- `.agents/skills/pruebas-funcionales/SKILL.md`
- `.agents/skills/costos/SKILL.md`
- `.agents/skills/integracion/SKILL.md`
- `.agents/skills/diseno-ux-ui/SKILL.md`

## Flujo
Descubrir → evaluar riesgos → plan mínimo → cambio en rama → pruebas disponibles → revisión humana → autorización expresa para integrar/desplegar.
