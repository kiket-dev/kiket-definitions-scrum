# Analytics overlays for Scrum template

The dbt project lives in the core Kikét repository, but this template adds
exposure metadata so customers can document dashboards directly in their Git repo.

- `exposures/delivery_health.yml` captures the Delivery Health dashboard and its
  dependencies (`fct_cycle_time`, `fct_throughput`, `fct_usage_events`).

Include this folder when publishing docs (`dbt docs generate`) so analytics assets
show alongside the rest of your project metadata.
