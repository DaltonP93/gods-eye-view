# Dalton Engineering capability update — 2026-11-24

GitHub Issues is disabled for this repository, so this file records the central capability-update notification.

Before substantial work, review:

- https://github.com/DaltonP93/Desarrollo/blob/main/docs/ADENDUM-CAPACIDADES-2026-11-24.md
- https://github.com/DaltonP93/Desarrollo/blob/main/docs/TOOL-CATALOG.md
- https://github.com/DaltonP93/Desarrollo/blob/main/docs/ADOPTION-MATRIX.md
- https://github.com/DaltonP93/Desarrollo/blob/main/profiles/catalog.yml

Classify relevant capabilities as **UTILIZAR AHORA / PILOTAR / FUTURO / NO APLICA**.

For gods-eye-view specifically, review design-system tooling and Storybook selectively; preserve the existing Three.js/3D pipeline and consider blender-skills only for genuine asset-pipeline needs. Observability/code-review additions are candidates, not automatic dependencies.

No deploy, dependency installation, infrastructure mutation or production action is authorized by this notice.


## Scalability and abrupt-growth update

Dalton Engineering now requires `scalability-resilience` for production-bound architecture.

For gods-eye-view, future architecture reviews must include:
- baseline/peak/10x/100x capacity assumptions;
- geospatial/3D asset and telemetry data growth;
- memory/GPU/CPU budgets and saturation;
- database/index/storage growth;
- bounded concurrency, queues and backpressure;
- load/spike/soak testing;
- HA, recovery and support/runbooks;
- runtime/language fitness and supported security lifecycle.

Central baseline:
https://github.com/DaltonP93/Desarrollo/blob/main/docs/SCALABILITY-RESILIENCE-BASELINE.md

Principle: scale-ready, not scale-overengineered. Do not introduce Kubernetes, sharding, microservices or a language rewrite without measured evidence.
