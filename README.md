# Operational_POD_health_monitoring_and_Alerting
Operation of POD health monitoring then Alerting script using python
Pod Alerting System

A lightweight Python tool that classifies Kubernetes pods by operational severity
and logs alerts based on platform reliability rules.

## Severity Model
- IGNORE: Platform-owned pods (handled by platform team)
- ESCALATE: Unhealthy status or severe restart storms
- INVESTIGATE: Moderate instability
- OK: Healthy pod

## Design Principles
- Explicit severity states (no ambiguous booleans)
- Deterministic decision logic
- Separation of classification and side effects
- Unit-testable core logic

## How to Run
```bash
python pod_alert.py
