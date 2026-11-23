# Fuentes, permisos y trazabilidad

Revisión: 16-11-2026. Único dataset real: [Online Retail II, UCI](https://archive.ics.uci.edu/dataset/502/online+retail+ii), Chen, DOI [10.24432/C5CG6D](https://doi.org/10.24432/C5CG6D). La ficha oficial consultada declara CC BY 4.0. Se puede compartir/adaptar con atribución y aviso de cambios; ver [licencia](https://creativecommons.org/licenses/by/4.0/) y NOTICE. No requiere cuenta ni scraping.

ZIP aprobado: 45.622.418 bytes, SHA-256 `572e36277c2390fbfde10664750731e0a86f55e33470d91919085f0408e67bfb`. XLSX aprobado: SHA-256 `bcbe73b35f5b7babf197fb0cb983a11f5d9ff929078d4aa53d171b1f2df2e980`. La ejecución actual reutilizó la descarga oficial comprobada el 11-11-2026, volvió a verificar ambos hashes y procesó las dos hojas completas. No se afirma una descarga nueva el 16-11.

Son transacciones británicas históricas de 2009–2011; la moneda es GBP y la hora original no tiene zona. No hay observaciones de pagos, costos o vencimientos. `Customer ID` es un identificador de la fuente: no se enriquece ni se interpreta como identidad de una persona. Los exports públicos de evidencia contienen agregados y muestras de trazabilidad, sin añadir datos personales.

La ingesta conserva líneas de contenido idéntico y genera identidad con checksum + hoja + fila. El libro original se mantiene fuera de Git; Parquet y PostgreSQL son derivados. Los cambios son normalización de nombres/tipos, clasificación por reglas explícitas y agregación. Cantidad negativa o prefijo C significa cancelación/corrección según las reglas, no un emparejamiento demostrado con una venta.

El fixture `data/fixtures/synthetic.xlsx` es original, reproducible con semilla 2026 y CC0. Su sidecar `.source.json` registra procedencia y hash; sin sidecar coherente, la ingesta sintética falla. Los incidentes de demo son inyectados. Nunca se mezclan con `retail_uk_reference`: tienen namespace `retail_synthetic`.

Contingencia: ZIP local con checksum aprobado; después, demo sintética que comprueba operación, sin sustituir la evaluación real. Un checksum real nuevo requiere revisión manual y nueva versión de la fuente. No se descarga un espejo distinto de forma silenciosa.

Los archivos de entrada se limitan a 80 MB al descargar/descomprimir el miembro esperado. No se extraen rutas arbitrarias de un ZIP. La caché Parquet también se verifica antes de reutilizarla. No hay credenciales de proveedores ni fuentes restringidas.
