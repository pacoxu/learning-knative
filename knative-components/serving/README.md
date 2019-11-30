# General Configs in Knative Serving

CRDs that you should know
- kubectl  api-resources | grep knative | grep serving
```
NAME                              SHORTNAMES      APIGROUP                           NAMESPACED   KIND
configurations                    config,cfg      serving.knative.dev                true         Configuration
revisions                         rev             serving.knative.dev                true         Revision
routes                            rt              serving.knative.dev                true         Route
services                          kservice,ksvc   serving.knative.dev                true         Service
```
- A Route provides a named endpoint and a mechanism for routing traffic to
- Revisions, which are immutable snapshots of code + config, created by a
- Configuration, which acts as a stream of environments for Revisions.
- Service acts as a top-level container for managing a Route and Configuration which implement a network service.

## Components
- kubectl get deployment -n knative-serving
```
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
activator          1/1     1            1           166m
autoscaler         1/1     1            1           166m
autoscaler-hpa     1/1     1            1           166m
controller         1/1     1            1           166m
networking-istio   1/1     1            1           166m
webhook            1/1     1            1           166m
```

You should learn about responsiblities of each components.

## Configurations
kubectl get configmap -n knative-serving -o yaml

### config-autoscaler
Knative concurrency-based autoscaling (default).
- autoscaling.knative.dev/class: kpa.autoscaling.knative.dev
- autoscaling.knative.dev/metric: concurrency
Target 10 requests in-flight per pod.
- autoscaling.knative.dev/target: "10"
Disable scale to zero with a minScale of 1.
- autoscaling.knative.dev/minScale: "1"
Limit scaling to 100 pods.
- autoscaling.knative.dev/maxScale: "100"
