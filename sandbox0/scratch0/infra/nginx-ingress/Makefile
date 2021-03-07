HELMREPO := https://helm.nginx.com/stable
RELEASE := nginx-ingress
VERSION := 0.8.0
CHART := nginx-ingress
NAMESPACE := infra

default:
	rm -rf manifests
	helm template \
	--output-dir manifests \
	--namespace $(NAMESPACE) \
	--values values.yaml \
	--repo $(HELMREPO) \
	--version $(VERSION) \
	--release-name $(RELEASE) \
	$(CHART)
