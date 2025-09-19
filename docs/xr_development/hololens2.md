# HoloLens 2 Development Guide

Deploying IRIS applications to HoloLens 2 requires tight coordination between Unity, MRTK, and device management tooling.

## Build Preparation

- Install the Mixed Reality Feature Tool and add MRTK 2.8+ packages to your project.
- Configure the Unity project for UWP with ARM64 architecture.
- Enable spatial perception, internet client, microphone, and research mode capabilities.

## Continuous Integration

1. Use `Unity -batchmode` to produce a UWP build.
2. Package the build with `msbuild /p:Configuration=Release`.
3. Upload the AppX bundle and dependency packages to the artifact store.

## Device Deployment

- Connect to the device via the Windows Device Portal and enable Developer Mode.
- Install certificates, then push the AppX bundle through the portal or using `Add-AppPackage` PowerShell commands.
- Confirm the app launches and connects to IRIS services in less than 10 seconds.

## Post-Deployment Validation

- Run MRTK diagnostics to ensure spatial mapping and hand tracking remain stable.
- Capture Mixed Reality Capture (MRC) footage for stakeholder review.
- Log issues and performance metrics in the IRIS deployment tracker.
