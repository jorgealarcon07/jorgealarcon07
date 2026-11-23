# Fuentes y procedencia

Todos los datos son sintéticos y pertenecen al namespace `payments_cop_synthetic`. El generador original y sus fixtures prescinden de datos personales, comerciantes reales, números de tarjetas, credenciales y extractos bancarios. Los datos generados se ofrecen bajo [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). El código del proyecto se ofrece bajo MIT.

Cada conjunto incluye facturas JSONL, catálogo de lotes, entregas JSONL y declaraciones CSV. El manifiesto registra semilla 2026 por defecto, licencia y SHA-256 de los cuatro archivos. El CSV se coteja por posición con las declaraciones emitidas en JSONL. La API local y los archivos exponen el mismo contrato. El fixture pequeño verificado se incluye en `data/fixtures/` y el oráculo manual vive en `tests/oracles/`.

La documentación de Stripe se consultó el 17-11-2026 como referencia de eventos repetidos, desorden, reintentos y reportes de liquidación. La simulación usa su propio esquema y reglas de completitud. [Entregas de eventos](https://docs.stripe.com/webhooks#event-delivery-behaviors) · [Reporte de conciliación](https://docs.stripe.com/reports/payout-reconciliation).
