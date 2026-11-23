# Jorge Alarcón

**Data Engineer · Data Scientist** | Físico con enfoque en sistemas complejos. [LinkedIn](https://www.linkedin.com/in/jorgealarconp/)

Trabajo con **Python y SQL** para construir procesos de datos confiables y evaluar decisiones con modelos y experimentos.

![Python](assets/stack/python.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg) ![dbt](assets/stack/dbt.svg) ![scikit-learn](assets/stack/scikitlearn.svg) ![MLflow](assets/stack/mlflow.svg)

## Proyectos

Faro es una empresa ficticia de comercio y pagos. Estos cuatro casos se pueden explorar por separado. [Ver los cuatro informes en el navegador](https://jorgealarcon07.github.io/jorgealarcon07/)

### [Cierre de ventas](https://github.com/jorgealarcon07/faro-data-foundation) · Data Engineering

**¿Qué ventas podemos dar por cerradas?** Construí un proceso que separa ventas, cancelaciones y ajustes, comprueba los totales y avisa a finanzas cuando faltan datos.

![Python](assets/stack/python.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg) ![dbt](assets/stack/dbt.svg) ![Parquet](assets/stack/apacheparquet.svg)

El cierre cuadró en 1.798 grupos de fecha y tipo de movimiento. De 1.067.371 filas, 243.007 carecían de cliente identificado, así que el informe quedó provisional.

[Ver el informe](https://jorgealarcon07.github.io/jorgealarcon07/cierre-de-ventas/) · [Explorar el proyecto](https://github.com/jorgealarcon07/faro-data-foundation)

### [Conciliación de pagos](https://github.com/jorgealarcon07/faro-reconciliation) · Data Engineering

**¿Qué abonos cuadran con lo que se cobró?** Construí una conciliación que compara cobros y abonos, reconoce mensajes repetidos y entrega a tesorería una lista de diferencias con su historial.

![Python](assets/stack/python.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg) ![API HTTP](assets/stack/http.svg) ![pytest](assets/stack/pytest.svg)

En una prueba de 100.000 entregas simuladas, detectó los 325 lotes con diferencias sembradas. Ninguno de esos lotes se marcó como conciliado.

[Ver el informe](https://jorgealarcon07.github.io/jorgealarcon07/conciliacion-de-pagos/) · [Explorar el proyecto](https://github.com/jorgealarcon07/faro-reconciliation)

### [Priorización de cuentas](https://github.com/jorgealarcon07/faro-risk-policy) · Data Science

**Si solo podemos revisar 300 cuentas, ¿por cuáles empezamos?** Construí una cola de revisión y comparé una regla de atraso con dos modelos. El equipo de riesgo puede ver qué cambia al dedicar más o menos revisiones.

![Python](assets/stack/python.svg) ![scikit-learn](assets/stack/scikitlearn.svg) ![MLflow](assets/stack/mlflow.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg)

Entre las primeras 300 de 6.000 cuentas de prueba hubo 232 impagos históricos con regresión logística, 227 con boosting y 215 con la regla de atraso.

[Ver el informe](https://jorgealarcon07.github.io/jorgealarcon07/revision-de-riesgo/) · [Explorar el proyecto](https://github.com/jorgealarcon07/faro-risk-policy)

### [Experimento de recordatorios](https://github.com/jorgealarcon07/faro-experiment-lab) · Data Science

**¿Vale la pena enviar otro recordatorio de pago?** Construí un ensayo A/B que mide pagos a 14 días, costo de envío y quejas. Operaciones recibe una recomendación y puede ver qué datos la sustentan.

![Python](assets/stack/python.svg) ![SciPy](assets/stack/scipy.svg) ![statsmodels](assets/stack/statsmodels.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg)

En el escenario favorable de 20.000 cuentas simuladas, el grupo asignado al recordatorio pagó 3,30 puntos porcentuales más. Al retirar 3.250 resultados, el sistema bloqueó la recomendación.

[Ver el informe](https://jorgealarcon07.github.io/jorgealarcon07/experimento-de-recordatorios/) · [Explorar el proyecto](https://github.com/jorgealarcon07/faro-experiment-lab)
