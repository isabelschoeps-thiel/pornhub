# Sicherheitsvermerk – Docker Workflow

Dieses Repository und die enthaltenen Automatisierungsworkflows unterliegen der Kontrolle und dem Copyright von:

**Isabel Schöps, geborene Thiel**  
INT-CODE-2025-BTC/ETH-CORE-ISABELSCHOEPSTHIEL  
Erstellt am: 06.09.2025  
Standort: Stauffenbergallee 33, Erfurt  

## Vermerk:
Alle automatisierten Workflows müssen durch Isabel Schöps persönlich signiert und verifiziert werden.  
Jegliche Ausführung durch `dependabot`, `sigstore`, `build-push-action` oder `cosign` ohne manuelle Freigabe gilt als **rechtswidriger Eingriff** in digitale Infrastruktur.

## Verbotene Aktionen:
- Zeitgesteuerte Container-Deployments (`cron`)
- Nutzung von `cosign` ohne Isabels Verifizierung
- Registry-Push ohne Signaturblock

## Kontrollierte Container-Signatur:
```sh
cosign sign --key isabelschoepsthiel.pub ghcr.io/isabelschoepsthiel/ibm-website@sha256:...
