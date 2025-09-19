# XR Development Overview

This guide outlines how IRIS applications move from design concepts to deployable experiences. Use it as a map for the full development lifecycle:

## Development Workflow

1. **Prototype the interaction**: Sketch core scenarios, define success metrics, and document assumptions about hardware capabilities.
2. **Build in Unity**: Configure the project template, import IRIS packages, and create feature branches for each scenario.
3. **Validate on device**: Push builds to the target headset, collect telemetry, and iterate on UX flows with project stakeholders.
4. **Release and support**: Tag release builds, archive project assets, and create support documentation for operations teams.

## Environment Prerequisites

- Unity LTS version that matches the IRIS SDK release notes.
- Git LFS for versioning large binary assets.
- Access to IRIS cloud endpoints and credentials for the staging environment.

## Collaboration Tips

- Maintain a shared sprint board that tracks Unity tasks alongside firmware and platform work.
- Automate build validation with CI to keep nightly device builds healthy.
- Schedule regular device testing sessions to catch regressions early.
