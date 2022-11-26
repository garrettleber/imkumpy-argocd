# mattermost chat server

<https://docs.mattermost.com/install/install-kubernetes.html>

You will need to manually install the operator first

```bash
kubectl create ns mattermost-operator
kubectl apply -n mattermost-operator -f https://raw.githubusercontent.com/mattermost/mattermost-operator/master/docs/mattermost-operator/mattermost-operator.yaml
```

then apply secrets/ns, I have provided examples here, but also keep a copy of mine locally in `secrets/all.yml`

```bash
kubectl apply -f secrets/all.yaml
```
