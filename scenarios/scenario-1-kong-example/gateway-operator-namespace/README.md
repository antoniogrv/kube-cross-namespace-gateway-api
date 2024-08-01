Please refer to [the instructions](https://docs.konghq.com/gateway-operator/1.3.x/get-started/kic/install/) provided in the official documentation.

```bash
helm repo add kong https://charts.konghq.com
helm repo update kong

helm upgrade --install kgo kong/gateway-operator -n gateway-operator --create-namespace --set image.tag=1.3
```