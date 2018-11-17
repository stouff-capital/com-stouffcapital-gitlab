1. `kubectl create -f registry-auth-ingress.yaml` to retrieve a certificate
1. `kubectl create configmap docker-registry-auth-cm --from-file=auth_config.yml -n gitlab`
1. `kubectl create -f registry-auth.yaml`
1. `kubectl create configmap docker-registry-cm --from-file=config.yml -n gitlab`
1. `kubectl create -f registry.yaml`
1. `kubectl create -f registry-ingress-ingress.yaml`