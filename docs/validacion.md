# Casos de prueba propuestos

| Caso | Resultado esperado | Estado |
|---|---|---|
| Dos solicitudes simultáneas para un mismo turno | Una confirmación y un rechazo por conflicto | Pendiente |
| Cancelar y volver a reservar el turno | Se conserva el historial y se crea una nueva ocupación | Pendiente |
| Consultar la agenda de otro complejo | Acceso denegado | Pendiente |
| Reservar una fecha pasada | Rechazo sin persistir cambios | Pendiente |
