## OpenShift State Metrics to Kube State Metrics migration

This repository holds Kube State Metrics' `CustomResourceState`
configurations for redefining all collectors implemented in
OpenShift State Metrics so we can migrate from it, and
eventually sunset that, with minimal-to-no user-facing changes
on the metrics front whatsoever.

### ToDos

- Relabeling exposed metrics to remove Kube State Metrics'
  induced artefacts.
- Implement `ClusterResourceQuota` while combining the
  sub-metrics and relabeling them. Additionally, consider
  wrapping them in custom rules for further customization
  whenever and wherever needed.
