# Origen y permisos

La evaluación utiliza *Default of Credit Card Clients* de I-Cheng Yeh, publicado por UCI en 2016. La cohorte contiene 30.000 cuentas de tarjeta de Taiwán. Los seis meses de historia van de abril a septiembre de 2005. La variable de resultado indica impago en el siguiente mes. Los importes están en TWD. La licencia CC BY 4.0 permite redistribuir y adaptar con atribución. [Ficha UCI](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients) · [DOI](https://doi.org/10.24432/C55S3H) · [Licencia](https://creativecommons.org/licenses/by/4.0/)

La entrada autorizada es el [ZIP oficial](https://archive.ics.uci.edu/static/public/350/default+of+credit+card+clients.zip), de 5.539.494 bytes, SHA-256 `56c885f84457f6680f8438f02bfcdac9579323d8a94465ee5f26e32baa727602`. El adaptador abre el miembro XLS por nombre, la hoja Data y el segundo encabezado. La copia local verificada por la misma huella sirve para trabajar sin red. Un cambio de huella exige revisar procedencia y esquema. El ZIP original se excluye de Git.

Las transformaciones incluyen ratios, conteos de atrasos, particiones de IDs, aprendizaje supervisado, scores y agregación. Los cierres de mes son convenciones analíticas. La fuente carece de instantes operativos de disponibilidad de etiquetas. El monitor de demora representa un calendario simulado.

El fixture de la demo contiene cuentas inventadas con semilla 2026. Cuatro columnas se generan a partir de distribuciones marginales de entrenamiento, con sorteos independientes. Las demás provienen de un generador. Conservamos atribución UCI para esta derivación. El fixture valida contratos, entrega y recuperación. Las cifras de desempeño provienen exclusivamente del holdout real.
