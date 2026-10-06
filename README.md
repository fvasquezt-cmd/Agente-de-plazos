# Libro de Plazos

Gestor gratuito de causas y plazos procesales para Chile. Funciona en el navegador, sin registro y sin servidor.

## Qué hace

- Registra causas: rol, carátula, tribunal, materia, cliente y notas.
- Calcula vencimientos desde la fecha de notificación en días hábiles (lunes a sábado o lunes a viernes), días corridos o meses, descontando feriados nacionales 2026 y 2027.
- Muestra la fecha alternativa cuando el tratamiento del sábado cambia el resultado.
- Ordena todo en un semáforo de urgencia: vencido, vence hoy, ≤ 2 y ≤ 5 días hábiles.
- Exporta los plazos pendientes a un archivo `.ics` con avisos 3 días y 1 día antes, importable en Google Calendar, Outlook o el calendario del teléfono.
- Descarga y restaura respaldos en JSON.
- Permite agregar feriados regionales o días inhábiles propios.

## Privacidad

Los datos se guardan solo en el navegador de cada usuario (`localStorage`). Nada se envía a ningún servidor. Si se borran los datos de navegación o se cambia de equipo, las causas se pierden, salvo que se haya descargado un respaldo.

## Publicar en GitHub Pages

1. Crea un repositorio público en GitHub, por ejemplo `libro-de-plazos`.
2. Sube `index.html` y este `README.md` con **Add file → Upload files** y confirma con **Commit changes**.
3. Ve a **Settings → Pages**. En **Source** elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
4. En uno o dos minutos la app queda disponible en `https://TU-USUARIO.github.io/libro-de-plazos/`.

## Mantenimiento

Los feriados están en la constante `FERIADOS_BASE` dentro de `index.html`. Actualízala cada año con el calendario oficial. El Día Nacional de los Pueblos Indígenas de 2027 está marcado como pendiente de verificación.

## Aviso

Herramienta de apoyo. No reemplaza la revisión del abogado ni constituye asesoría legal. Cada usuario debe verificar el cómputo según la norma aplicable al procedimiento (feria judicial, aumento por tabla de emplazamiento, plazos especiales). El autor no responde por plazos mal calculados ni por datos perdidos.
