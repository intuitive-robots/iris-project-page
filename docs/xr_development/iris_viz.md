# IRIS-Viz Unity Setup

Follow these steps to configure the IRIS-Viz Unity project for XR development.

## 1. Install Dependencies

- Unity LTS with Android and UWP build support.
- XR Interaction Toolkit (latest verified package).
- IRIS SDK `.unitypackage` file from the developer portal.

## 2. Create the Project

1. Start a new 3D (URP) project.
2. Set the Company Name and Product Name to match the IRIS deployment manifest.
3. Add the project folder to source control and enable Git LFS for `*.psd`, `*.fbx`, and `*.unitypackage` assets.

## 3. Configure Build Settings

- Switch the active build target to the intended headset (Android for Quest, UWP for HoloLens).
- Enable Virtual Reality support and add the appropriate XR plugin.
- Set the minimum API level and scripting backend based on platform certification requirements.

## 4. Import IRIS Assets

1. Import the IRIS SDK package.
2. Open the Sample Scene and confirm no compilation errors.
3. Configure the `IrisAppConfig` ScriptableObject with environment endpoints and API keys.

## 5. Verify the Setup

- Run Play Mode tests in the editor to validate the interaction prefabs.
- Trigger a test build and deploy to the target device.
- Capture performance metrics using Unity Profiler or the device-specific tooling.
