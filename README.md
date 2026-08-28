# PreflightOps pull-request demo

This repository is a small, runnable example of PreflightOps `v0.3.0` reviewing
a production change in GitHub Actions.

The example demonstrates:

- a service catalog and structured change request;
- changed-file detection for Terraform and Kubernetes;
- a compact, idempotent pull-request comment;
- Markdown, JSON, and static HTML review artifacts; and
- an advisory `HIGH` result that passes a `CRITICAL` blocking threshold.

See the repository's example pull request for the complete check and comment.

## Files

- `services.yaml`: service ownership and criticality.
- `change.yaml`: rollback, monitoring, and validation evidence.
- `tfplan.json`: structured Terraform plan evidence.
- `tfplan.txt`: legacy human-readable plan example.
- `k8s.yaml`: Kubernetes workload evidence.
- `.github/workflows/preflightops.yml`: real pull-request workflow.

No cloud, ServiceNow, Jira, or other paid resources are created by this demo.
