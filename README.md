# kiket-definitions-scrum
Standard SCRUM definitions for Kiket.

## Analytics assets

Scrum projects inherit dbt-backed analytics assets:

- `.kiket/analytics/dashboards/delivery_health.yaml` tracks cycle time, throughput, and usage events with built-in alerts for regressions.
- `analytics/dbt/exposures/delivery_health.yml` documents the dashboard for `dbt docs` and lineage tooling.

Synchronise definitions and run the analytics pipeline to populate the underlying `analytics_org_*` schemas before exploring the dashboards in the product. When running `dbt docs generate`, include the exposure directory from this repository.
