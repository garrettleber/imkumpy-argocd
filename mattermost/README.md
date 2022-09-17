https://docs.mattermost.com/install/install-kubernetes.html

You will need to manually install the operator first

```bash
kubectl create ns mattermost-operator
kubectl apply -n mattermost-operator -f https://raw.githubusercontent.com/mattermost/mattermost-operator/master/docs/mattermost-operator/mattermost-operator.yaml
```