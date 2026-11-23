# Jorge Alarcón

**Data Engineer · Data Scientist** | Physicist with a focus on complex systems. [Español](README.es.md) · [LinkedIn](https://www.linkedin.com/in/jorgealarconp/)

I use **Python and SQL** to build reliable data pipelines and evaluate decisions with models and experiments.

![Python](assets/stack/python.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg) ![dbt](assets/stack/dbt.svg) ![scikit-learn](assets/stack/scikitlearn.svg) ![MLflow](assets/stack/mlflow.svg)

## Projects

I built four independent projects for Faro, a fictional retail and payments company. [Explore the portfolio in English](https://jorgealarcon07.github.io/jorgealarcon07/en/)

### [Sales close](https://github.com/jorgealarcon07/faro-data-foundation) · Data Engineering

**Which sales figures are ready to use?** I built a pipeline that separates sales, cancellations and adjustments, checks the totals and flags missing data for the finance team.

![Python](assets/stack/python.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg) ![dbt](assets/stack/dbt.svg) ![Parquet](assets/stack/apacheparquet.svg)

The totals matched an independent calculation across 1,798 groups of transactions by date and type. Of 1,067,371 historical rows, 243,007 lacked a customer ID, so the close was published as provisional.

[Case study](https://github.com/jorgealarcon07/faro-data-foundation/blob/main/CASE_STUDY.md) · [Interactive report (Spanish)](https://jorgealarcon07.github.io/jorgealarcon07/cierre-de-ventas/)

### [Payment reconciliation](https://github.com/jorgealarcon07/faro-reconciliation) · Data Engineering

**Which processor payouts match the underlying payments?** I built a pipeline that reconciles payments and payouts, handles duplicate messages and gives treasury a queue of discrepancies to investigate.

![Python](assets/stack/python.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg) ![HTTP API](assets/stack/http.svg) ![pytest](assets/stack/pytest.svg)

In a test with 100,000 simulated event deliveries, the pipeline detected all 325 payout batches with deliberately introduced discrepancies and kept them open.

[Case study](https://github.com/jorgealarcon07/faro-reconciliation/blob/main/CASE_STUDY.md) · [Interactive report (Spanish)](https://jorgealarcon07.github.io/jorgealarcon07/conciliacion-de-pagos/)

### [Account review prioritization](https://github.com/jorgealarcon07/faro-risk-policy) · Data Science

**If the risk team can review only 300 accounts, where should it start?** I built a review queue and compared an overdue-payment rule with two models at different review capacities.

![Python](assets/stack/python.svg) ![scikit-learn](assets/stack/scikitlearn.svg) ![MLflow](assets/stack/mlflow.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg)

Among the first 300 of 6,000 historical test accounts, logistic regression surfaced 232 observed defaults, gradient boosting surfaced 227 and the overdue-payment rule surfaced 215.

[Case study](https://github.com/jorgealarcon07/faro-risk-policy/blob/main/CASE_STUDY.md) · [Interactive report (Spanish)](https://jorgealarcon07.github.io/jorgealarcon07/revision-de-riesgo/)

### [Payment reminder experiment](https://github.com/jorgealarcon07/faro-experiment-lab) · Data Science

**Is an extra payment reminder worth sending?** I built an A/B test that measures payment within 14 days, messaging costs and complaints, then gives operations a recommendation backed by those results.

![Python](assets/stack/python.svg) ![SciPy](assets/stack/scipy.svg) ![statsmodels](assets/stack/statsmodels.svg) ![SQL · PostgreSQL](assets/stack/postgresql.svg)

In a favorable scenario with 20,000 simulated accounts, those assigned a reminder paid at a rate 3.30 percentage points higher. Removing 3,250 outcomes caused the system to block the recommendation.

[Case study](https://github.com/jorgealarcon07/faro-experiment-lab/blob/main/CASE_STUDY.md) · [Interactive report (Spanish)](https://jorgealarcon07.github.io/jorgealarcon07/experimento-de-recordatorios/)
