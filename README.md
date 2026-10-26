# Winflex · Mantenimiento

App de una sola página para registrar los gastos de mantenimiento y seguir los proyectos de planta (planeamiento, puesta en marcha, seguimiento). Mismo diseño, logo y esquema de PIN que el resto de las apps Winflex.

## Módulos
- **Dashboard**: gasto del mes, acumulado del año vs. mismo período del año anterior (U$D), promedio mensual, gasto mensual apilado por sector, Pareto de equipos, proveedores, categorías y tipo de intervención. Todo en U$D (oficial de cada fecha) o en pesos.
- **Gastos**: carga con fecha, planta, sector, equipo, descripción, detalle de lo hecho, tipo (correctivo / preventivo / mejora / proyecto), categoría, proveedor, factura, importe, TC, tipo de pago B/N, horas de máquina parada, responsable y proyecto/etapa. Filtros y exportación a Excel (CSV).
- **Proyectos**: tablero por estado (idea → evaluación → aprobado → ejecución → puesta en marcha → cerrado). Cada proyecto tiene ficha (objetivo, justificación, presupuesto, ahorro esperado → repago), etapas con fechas, presupuesto y tareas (cronograma tipo Gantt), checklist de puesta en marcha, bitácora y gastos reales vinculados.
- **Equipos y proveedores**: gasto por equipo (12 meses / histórico / horas de parada) y ranking de proveedores.
- **A revisar**: proyectos atrasados o pasados de presupuesto, etapas vencidas y gastos incompletos.

## Datos
Trae precargada la planilla "5-Costos Mantenimiento General E41" (492 gastos jun-2022 → oct-2026). Se guardan en JSONBin (misma cuenta que las otras apps). La primera vez, Matías entra y toca **Crear base en la nube**; el ID que muestra se deja fijo en `BIN_FIJO`.

TC: oficial BNA venta por fecha (api.argentinadatos.com). Los gastos de la planilla hasta 2025 conservan su propio TC.

## Usuarios
PINs en la constante `USUARIOS` (Matías admin, Juan Manuel / Jonathan / Agustín carga, Mirta lectura).
