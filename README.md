# Azúcar OS

Sistema de gestión para Azúcar Dance Studio: membresías, acceso facial y torniquete, CRM y campañas, finanzas, profesores, staff, sucursales y salones.

## Estado

**Fase 0 · Prototipo navegable.** Un solo archivo HTML con datos de ejemplo para validar pantallas y flujos antes de construir el sistema real.

- `prototipo/index.html` — ábrelo en el navegador e inicia sesión con una de las cuentas de prueba (contraseña `demo2026`). Cada perfil ve solo lo que le corresponde.
- El inicio de sesión del prototipo es una simulación: no protege nada. En el sistema real las contraseñas se guardan cifradas en el servidor, con recuperación por correo y bloqueo por intentos fallidos.
- Los alumnos del prototipo son ficticios. Los precios y reglas vienen de los flyers ADS 2026.
- La identidad visual sigue el Manual de marca v1.0 (octubre 2026).

## Perfiles de acceso

| Perfil | Ve |
|---|---|
| Socio / Dirección | Todo: dashboard, finanzas, marketing, CRM, staff, configuración |
| Staff · Recepción | Su turno y corte de caja, ventas del día, check-in, alumnos e historial de membresía, agenda, punto de venta, CRM. Sin KPIs financieros |
| Profesor | Su agenda, lista de asistencia (solo nombres), sus calificaciones y videos de capacitación |
| Alumno | La app: pase de acceso, pago, reservas, calificar clases y suscripción de videos |

## Plan

1. **Fase 0** · Prototipo navegable (este repositorio).
2. **Fase 1** · Alumnos, paquetes, pagos, check-in por QR, dashboard básico. Migración de la base de GymForce.
3. **Fase 2** · CRM, campañas por WhatsApp Business API y app del alumno (PWA).
4. **Fase 3** · Terminal facial ZKTeco y torniquete, calificación de profesores, evaluación de staff, capacitación en video.
5. **Fase 4** · Facturación CFDI con Facturama y reportes avanzados.

Stack propuesto para el sistema real: Next.js + PostgreSQL, desplegado en el servidor de CloudPanel.

## Datos personales

Nunca subir a este repositorio exportes de GymForce, listas de clientes ni datos biométricos. Ver `.gitignore`.
