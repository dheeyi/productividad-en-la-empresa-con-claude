# Módulo 1 — Prompts y pasos

> Prompts para copiar, en el orden de las clases.
> Curso: **Productividad en la empresa con Claude** · plan de referencia: **Claude Pro** · octubre 2026.
> Archivos de práctica: descarga `practica-modulo-1.zip` (carpeta `assets/`), descomprímelo y dale acceso a Claude a la carpeta `modulo-1`.
> Un **prompt** es el mensaje que le escribes a Claude.

---

## Clase 1 · El problema de las empresas
*Deja de ir directo a ejecutar: primero planifica.*

▸ Prompt “directo a ejecutar” (lo que NO conviene hacer):
```
Limpia este Excel.
```

▸ Prompt con método (primero el plan):
```
Antes de hacer nada, dame un plan paso a paso para limpiar ventas-q3.xlsx.
No modifiques el archivo todavía.
```

> El método: **planificar → ejecutar → revisar → iterar**.

---

## Clase 2 · Modos de trabajo en Claude Desktop
*Prepara tu espacio: carpeta local o conectores.*

▸ Descarga Claude Desktop (macOS o Windows): https://claude.com/download

▸ Activa la creación de archivos en la configuración de Claude: opción **ejecución de código y creación de archivos**
  (en la documentación en inglés: *Settings › Capabilities › Code execution and file creation*).

▸ Antes de empezar, guarda aparte una copia de la carpeta `modulo-1`: si algo sale mal, vuelves a empezar con ella.

▸ Modo carpeta local: en la caja de mensaje elige la carpeta `modulo-1` y escribe:
```
Revisa esta carpeta y dime qué contiene cada archivo.
```

▸ Privacidad: revisa en la configuración la opción **Privacidad › Ayudar a mejorar Claude**.
  En planes de empresa (Team) tus datos no se usan para entrenar.

▸ Modo conectores (solo lo vemos, no lo practicamos): **Personalización › Conectores**.
> Microsoft 365 (Outlook, OneDrive) requiere una cuenta de trabajo.

> **Nuevo en 2026:** Chat y Cowork son una sola pestaña. Cowork trabaja en la nube:
> para usar tu carpeta local, **deja la app abierta**.

---

## Clase 3 · Excel: valida, limpia y actualiza
*Datos limpios y al día, sin hacerlo a mano.*

▸ (Opcional, solo demostración) generar una hoja de ejemplo:
```
Crea una hoja de Excel con 50 ventas de ejemplo que tenga errores típicos:
duplicados, celdas vacías y fechas en distintos formatos.
```

▸ Planifica (diagnóstico, sin tocar nada):
```
Revisa ventas-q3.xlsx y dime qué está mal antes de corregir nada.
Agrupa los problemas por tipo y dime cuántas filas afecta cada uno.
```

▸ Limpia y valida:
```
Aplica el plan sobre una copia llamada ventas-q3-limpio.xlsx (no toques el original):
- elimina las filas duplicadas,
- unifica las fechas en formato dd/mm/aaaa,
- deja el Estado solo como "Pagado" o "Pendiente",
- corrige los nombres de clientes y regiones mal escritos,
- no inventes datos: marca las celdas vacías en una columna "Revisar".
```

▸ Actualiza un Excel con los datos de otro (lo que harías con **BUSCARV**).
Primero el diagnóstico, sin cambios:
```
Quiero actualizar el Estado de ventas-q3-limpio.xlsx con pagos-actualizados.xlsx,
cruzando por la columna ID. Antes de cambiar nada, dime:
cuántos IDs coinciden, cuántos no, y cuántas filas cambiarían de estado.
No modifiques el archivo todavía.
```

▸ Después, aplícalo y deja marcadas las filas que cambiaron:
```
Aplícalo y guarda los cambios en el mismo ventas-q3-limpio.xlsx (no crees otro archivo).
Agrega al final una columna "Cambió" que diga "Sí" en las filas que actualizaste,
y dime cuántas filas cambiaron.
```

▸ Revisa el resultado:
```
Compara ventas-q3.xlsx con ventas-q3-limpio.xlsx: ¿cuántas filas había,
cuántas quedaron y por qué? ¿Se perdió algún dato que no debía perderse?
```

---

## Clase 4 · Convierte entre formatos
*De Excel a PowerPoint y a un reporte ejecutivo.*

▸ Planifica la presentación:
```
Con ventas-q3-limpio.xlsx, propón los 5 insights que pondrías en una
presentación para gerencia. No crees nada todavía.
```

▸ De Excel a PowerPoint:
```
Con ventas-q3-limpio.xlsx arma 5 diapositivas con los insights clave.
Una idea por diapositiva y un gráfico donde ayude. Por ahora no uses ninguna plantilla.
Guárdalo como reporte-q3.pptx dentro de una carpeta nueva llamada reporte-q3.
```

> **En Mac:** ábrelo con PowerPoint (instalado o gratis en office.com) o súbelo a Google Slides. La vista rápida y Keynote pueden mostrar los gráficos en blanco.

▸ Itera el resultado:
```
En la diapositiva de regiones, cambia el gráfico por uno de torta
con el % de ventas de cada región, y acorta los textos a una línea.
```

▸ De Excel o Word a un reporte ejecutivo:
```
Con informe-base.docx y ventas-q3-limpio.xlsx crea un reporte ejecutivo
de una página en PDF: resumen, 3 cifras clave y próximos pasos.
Tampoco uses la plantilla todavía. Guárdalo en la carpeta reporte-q3 como reporte-ejecutivo.pdf.
```

▸ Revisa las cifras (no confíes a ciegas):
```
Muéstrame cómo calculaste el porcentaje de ventas del Centro.
```

▸ Trabaja sobre tu plantilla:
```
Ahora rehaz reporte-q3.pptx y reporte-ejecutivo.pdf usando plantilla-empresa.pptx:
sus colores, su tipografía y su logo. Guárdalos en la carpeta reporte-q3
como reporte-q3-empresa.pptx y reporte-ejecutivo-empresa.pdf.
```

> **Nuevo en 2026:** Claude Slides (beta) también crea presentaciones que se descargan en PowerPoint o PDF.

---

## Clase 5 · Deja el copia y pega
*De uno a cien documentos, desde tu plantilla.*

▸ Prepara y entiende los archivos:
```
Revisa plantilla-contrato.docx y listado-clientes.xlsx: ¿qué campos hay que
reemplazar y de qué columna sale cada uno?
```

▸ Planifica las reglas:
```
Reglas: {{monto}} con separador de miles y 2 decimales;
{{fecha}} en formato largo (por ejemplo, 5 de julio de 2026).
Muéstrame el plan antes de generar nada.
```

▸ Genera el primer documento y revísalo:
```
Genera solo el contrato de Acme S.A. para revisarlo.
```

▸ Genera todos desde el listado:
```
Genera un documento por cada cliente del listado usando mi plantilla.
Guárdalos en una carpeta contratos/ con el nombre contrato-<cliente>.docx.
```

▸ Revisa antes de enviar:
```
Revisa los 24 contratos: ¿quedó algún {{campo}} sin reemplazar, algún monto
vacío o alguna fecha mal escrita? Dame una lista.
```
