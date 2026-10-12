# Módulo 2 — Prompts y pasos

> Prompts para copiar, en el orden de las clases.
> Curso: **Productividad en la empresa con Claude** · plan de referencia: **Claude Pro** · octubre 2026.
> Archivos de práctica: descarga `practica-modulo-2.zip` (carpeta `assets/`), descomprímelo y dale acceso a Claude a la carpeta `modulo-2`.

---

## Clase 1 · De la prueba y error a la Skill
*Escribe tu procedimiento una sola vez.*

▸ Activa las Skills: en la configuración de Claude, opción **ejecución de código y creación de archivos**.
Las ves y activas en **Personalización › Skills**.

▸ Conoce lo que ya tienes:
```
¿Qué Skills tengo disponibles y para qué sirve cada una?
```

> **Skill** = un procedimiento que se repite · **Proyecto** = el contexto de un tema ·
> **Instrucción** = algo puntual, una sola vez.

▸ Lo que pides SIEMPRE (por ejemplo, fechas en dd/mm/aaaa) va en la configuración → **preferencias personales**.

---

## Clase 2 · Dashboard en Excel
*De datos crudos a un tablero claro.*

▸ Planifica las métricas:
```
Con datos-crudos.xlsx propón 4 métricas clave antes de armar el dashboard.
Explica qué pregunta responde cada una.
```

▸ Ejecuta:
```
Crea dashboard-ventas.xlsx con una hoja "Dashboard": las 4 métricas arriba,
un gráfico de ventas por región y el top 5 de clientes.
```

▸ Itera:
```
Cambia el gráfico de región a barras horizontales, usa una sola paleta
de colores y ordena las métricas de mayor a menor importancia.
```

▸ Cuándo parar:
```
Revisa el dashboard: ¿responde las 4 preguntas del plan?
Si las responde, no cambies nada más.
```

---

## Clase 3 · Crea tu Skill
*Convierte la conversación en un procedimiento.*

▸ En la misma conversación del dashboard:
```
Convierte lo que acabamos de hacer en una Skill reutilizable
llamada dashboard-ventas.
```

▸ Revisa qué lleva dentro:
```
Antes de guardarla, muéstrame el nombre, la descripción y los pasos de la Skill.
```

▸ La descripción manda:
```
Mejora la descripción para que se active cuando pida un dashboard de ventas
a partir de un Excel con datos crudos.
```

▸ Guarda la Skill y confirma en **Personalización › Skills** que aparece activada.
> Al usarla verás **«Using dashboard-ventas»** en la respuesta de Claude.

---

## Clase 4 · Pon tu Skill a prueba
*Valida, corrige y afínala hasta que quede lista.*

▸ Pruébala con un archivo distinto:
```
Usa la Skill dashboard-ventas con ventas-q4.xlsx y dime qué no pudo resolver.
```

▸ Indica los cambios y actualiza la Skill:
```
Actualiza la Skill: si no encuentra la columna "Región", busca columnas
equivalentes como "Zona"; y si no está segura, que me pregunte.
```

▸ Segunda prueba:
```
Vuelve a usar la Skill dashboard-ventas con ventas-q4.xlsx.
```

> **¿Está terminada?** Funciona con otro archivo · no tienes que explicarle nada extra ·
> da el mismo resultado en 2 pruebas · su descripción dice cuándo usarla.

---

## Clase 5 · El resumen de los viernes
*Skill avanzada: el correo listo para enviar.*

▸ Conecta tu correo: **Personalización › Conectores › Gmail**.
> Si prefieres, practica con un correo de prueba en lugar de tu bandeja real.

▸ Planifica qué es importante:
```
Revisa mis correos de esta semana y dime cuáles son importantes
(clientes, pagos, plazos) y cuáles ignorarías. No redactes nada todavía.
```

▸ Construye e itera:
```
Escribe un borrador de correo "Resumen semanal" con lo importante:
viñetas, máximo 10 líneas. Déjalo como borrador, no lo envíes.
```

▸ Conviértelo en Skill:
```
Convierte este proceso en una Skill llamada resumen-viernes.
```

▸ Prográmala:
```
Cada viernes a las 9:00, resume mis correos de la semana en un borrador.
```
O desde **Programadas › Nueva tarea**: frecuencia semanal, viernes, 9:00.

> **Nuevo en 2026:** Gmail ya puede enviar correos, con tu aprobación en cada envío.
> En este curso elegimos dejarlo como borrador para revisarlo antes de enviar.
