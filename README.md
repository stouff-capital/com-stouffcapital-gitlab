1. `kubectl create -f gitlab/gitlab-namespace.yaml`

1. `kubectl create -f docker-registry/registry-auth-ingress.yaml`
1. `kubectl create configmap docker-registry-auth-cm --from-file=docker-registry/auth_config.yml -n gitlab`
1. `kubectl create -f docker-registry/registry-auth.yaml`

1. `kubectl create -f docker-registry/registry-pvc.yaml`
1. `kubectl create configmap docker-registry-cm --from-file=docker-registry/config.yml -n gitlab`
1. `kubectl create -f docker-registry/registry.yaml`
1. `kubectl create -f docker-registry/registry-ingress.yaml`


1. `kubectl create -f gitlab/gitlab-secret.yaml`
1. `kubectl create -f gitlab/gitlab-cm-common.yaml`
1. `kubectl create -f gitlab/gitlab-cm-https.yaml`
1. `kubectl create -f gitlab/gitlab-cm-oauth.yaml`
1. `kubectl create -f gitlab/gitlab-postgresql-pvc.yaml`
1. `kubectl create -f gitlab/gitlab-redis-pvc.yaml`
1. `kubectl create -f gitlab/gitlab-ce-pvc.yaml`
1. `kubectl create -f gitlab/gitlab-postgresql.yaml`
1. `kubectl create -f gitlab/gitlab-redis.yaml`
1. `kubectl create -f gitlab/gitlab-ce.yaml`
1. `kubectl create -f gitlab/gitlab-ingress-https.yaml`


1. `kubectl create -f gitlab/gitlab-ci-runner/gitlab-ci-runner-namespace.yaml`
1. `kubectl create -f gitlab/gitlab-ci-runner/gitlab-ci-runner-secret.yaml`
1. `kubectl create -f gitlab/gitlab-ci-runner/gitlab-ci-runner-rbac.yaml`
1. `kubectl create -f gitlab/gitlab-ci-runner/gitlab-ci-runner-configmap.yaml`
1. `kubectl create -f gitlab/gitlab-ci-runner/gitlab-ci-runner.yaml`

