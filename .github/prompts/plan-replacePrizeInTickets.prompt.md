# Plan: Reemplazar premio en tickets de rifa

## TL;DR
Cambiar el premio en los tickets de rifa de "1 Pollo Hornado" a "1 Gallina Picomocho Despresada". Hay una única línea que modificar en el código JavaScript.

## Steps
1. Reemplazar el texto en la línea 414 del archivo, cambiando `'  <div class="t-prize">&#8226; 1 Pollo Hornado</div>';` a `'  <div class="t-prize">&#8226; 1 Gallina Picomocho Despresada</div>';`
2. Verificar que el cambio aparece correctamente en la vista previa al generar los tickets

## Relevant files
- [index.html](index.html#L414) — Función `createTicket()` que genera el contenido del ticket (línea 414)

## Verification
1. Generar al menos 1 ticket desde el panel de control presionando "Generar Tickets"
2. Verificar en la vista previa que donde antes decía "1 Pollo Hornado" ahora dice "1 Gallina Picomocho Despresada"
3. Imprimir un ticket para confirmar que se ve correctamente en la salida impresa

## Decisions
- Solo se reemplaza en la sección del premio del ticket (no hay otros lugares donde aparece el texto)
- El formato y estructura del ticket permanece igual, solo cambia el nombre del premio
