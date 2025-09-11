# Installation

Instructions for installing the IRIS project and its dependencies.


## SimPublisher Installation

**SimPublisher** is the Python library for using IRIS.

Currently, You can install it by cloning the repository and setting it up in your Python environment.

**Step 1. Install dependencies**

```bash
pip install zmq trimesh
```

**Step 2. Clone the repository**

```bash
git clone git@github.com:intuitive-robots/SimPublisher.git
```

**Step 3. Install SimPublisher**

```bash
cd path/to/SimPublisher
pip install -e .
```

**Note:** SimPublisher will be published to PyPI in the future, making installation simpler.


## Deploy on XR Headsets

Currently, **IRIS** supports the following XR devices:  

### Supported Devices and Deployment

| Platform | Motion Controller | Hand Tracking | Gaze Tracking | Deployment Guide |
|----------|------------------|---------------|---------------|---------------|
| [Meta Quest 3](https://www.meta.com/quest/quest-3/) | ✅ | ✅ | ❌ | [Deploy on Meta Quest 3](../xr_application/meta_quest3.md) |
| [Microsoft HoloLens 2](https://www.microsoft.com/en-us/hololens) | ❌ | ✅ | ✅ | [Deploy on HoloLens 2](../xr_application/hololens2.md) |



