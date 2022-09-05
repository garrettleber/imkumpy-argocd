# loki, grafana, prometheus, and promtail stack
https://medium.com/nerd-for-tech/logging-at-scale-in-kubernetes-using-grafana-loki-3bb2eb0c0872

### Getting the Load Balancer IP 

kubectl get svc loki-stack-grafana -o jsonpath='{.status.loadBalancer.ingress[0].ip}' -n loki-stack


### Getting the admin username and Password 

kubectl get secret loki-stack-grafana -o go-template='{{range $k,$v := .data}}{{printf "%s: " $k}}{{if not $v}}{{$v}}{{else}}{{$v | base64decode}}{{end}}{{"\n"}}{{end}}' -n loki-stack