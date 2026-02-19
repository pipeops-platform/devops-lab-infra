# Infrastructure Runbook

## Provisioning Flow

1. Run Terraform format and validation
2. Execute Terraform plan
3. Apply approved infrastructure changes
4. Run Ansible playbooks for host configuration
5. Validate host and cluster readiness

## Troubleshooting

- If Terraform plan is unexpected, review drift and variable inputs.
- If Ansible fails, rerun with verbose output and verify inventory/credentials.

## Definition of Done

Provisioning and configuration complete successfully with validated infrastructure state.
