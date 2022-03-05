# Buoyant-Cloud


## Installation

### Create namespace
```bash
kubectl create ns buoyant-cloud
```

### Install the buoyant-cloud extension
```bash
curl --proto '=https' --tlsv1.2 -sSfL https://buoyant.cloud/install | sh # get the installer
linkerd buoyant install | kubectl apply -f - # connect to the hosted metrics stack
```
### Once you’ve installed your extensions, let’s validate
```bash
linkerd check
```

### Access Buoyant dashboard
```bash
linkerd buoyant dashboard &
```
