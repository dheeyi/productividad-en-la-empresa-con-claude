# Módulo 2 — Prompts y pasos

> Prompts para copiar, en el orden de las clases.
> Curso: **Productividad en la empresa con Claude** · plan de referencia: **Claude Pro** · octubre 2026.
> Archivos de práctica: descarga `practica-modulo-2.zip` (carpeta `assets/`) y descomprímelo.
> En este módulo trabajas en un **proyecto**: créalo y agrégale dos carpetas, `modulo-1` (la que usaste en el Módulo 1) y `modulo-2`.
> Un proyecto puede usar varias carpetas a la vez. Cuando pidas un archivo, di en qué carpeta guardarlo.

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

▸ Mira una Skill en acción:
```
Cada trimestre preparo el reporte de ventas así:
1. Limpio el Excel de ventas: duplicados, fechas y estados.
2. Actualizo los pagos con el Excel de Finanzas.
3. Saco los 5 insights para gerencia.
4. Armo la presentación en PowerPoint: una idea por diapositiva y un gráfico de torta por región.
5. Hago el informe ejecutivo en PDF, de una página: resumen, 3 cifras clave y próximos pasos.
6. Paso la presentación y el informe a la plantilla de la empresa.
Ponlo en un documento de Word de una página, claro y ordenado como procedimiento.
Guárdalo en la carpeta modulo-2 como pasos-reporte-ventas.docx.
```
Fíjate en el aviso **«Using docx»**: Claude usó la Skill de Word solo, sin que se lo pidieras.

▸ *Opcional:* para que Claude siempre te diga qué Skill usó, agrega esto en **preferencias personales**:
```
Cuando uses una Skill, indica siempre cuál usaste en cada paso y en la respuesta final.
```

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
Crea dashboard-ventas.xlsx en la carpeta modulo-2 con una hoja "Dashboard": las 4 métricas arriba,
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
llamada dashboard-ventas. Que siempre guarde el dashboard en la misma carpeta del Excel que le paso.
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
Escribe un borrador de correo "Resumen semanal" dirigido a mí mismo, con lo importante:
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

▸ Los contratos del Módulo 1, por correo (usa la carpeta `modulo-1` del proyecto):
```
Con listado-clientes.xlsx y los contratos de la carpeta modulo-1/contratos,
prepara un correo para cada cliente: dirigido a su Contacto, a su Correo,
con su contrato adjunto. Muéstrame cómo quedaría el de Acme S.A. antes de crear nada.
```

▸ Prueba con uno y revísalo en Gmail:
```
Crea solo el borrador de Acme S.A. en Gmail, con su contrato adjunto. No lo envíes.
```

▸ Conviértelo en Skill:
```
Convierte este proceso en una Skill llamada correos-contratos.
Que siempre deje los correos como borrador y nunca los envíe.
```

▸ Úsala con varios clientes:
```
Usa la Skill correos-contratos con Nova Ltda., Delta y Grupo Sur.
```

> **Nuevo en 2026:** Gmail ya puede enviar correos, con tu aprobación en cada envío.
> En este curso elegimos dejarlo como borrador para revisarlo antes de enviar.
