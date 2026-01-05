# Lead Radar Config (GitOps)

This repo is the **source of truth** for Lead Radar configuration.

It is deployed to Kubernetes via Argo CD as a `ConfigMap` in the `lead-radar` namespace.

## Files

- `k8s/lead-radar-configmap.yaml`: ConfigMap holding runtime configuration files.
- `schema/lead-radar-config.schema.json`: JSON Schema for the config payloads.

## Notes

- This repo is intended to be edited by an ERPNext UI (direct commits to `main`) and applied by Argo CD.
- Configuration is **public-data only** (RSS/feeds/news), no paid enrichment.

