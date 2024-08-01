```
{namespace} gateway-operator
├─ Gateway CRDs
├─ [Other objects...]

{namespace} gateway-01
├─ GatewayConfiguration
├─ GatewayClass
├─ Gateway
├─ HTTPRoutes
    ├─ application-01-httproute
    ├─ application-02-httproute

{namespace} application-01 [exposed via gateway-01]
├─ Service
├─ Deployment
├─ [Other objects...]
├─ ReferenceGrant
    ├─ application-01-httproute-grant

{namespace} application-02 [exposed via gateway-01]
├─ Service
├─ Deployment
├─ [Other objects...]
├─ ReferenceGrant
    ├─ application-02-httproute-grant

```