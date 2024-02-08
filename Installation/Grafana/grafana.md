# Install Grafana using Helm

```sh
helm repo add grafana https://grafana.github.io/helm-charts
helm repo update
helm install grafana grafana/grafana
kubectl expose service grafana — type=NodePort — target-port=3000 — name=grafana-ext
```