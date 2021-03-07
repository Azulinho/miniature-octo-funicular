HELMREPO := https://kubernetes.github.io/ingress-nginx
RELEASE := ingress-nginx-controller
VERSION := 3.23.0
CHART := ingress-nginx

default:
	rm -rf templates/
	helm template \
	--output-dir templates/ \
	--values values.yaml \
	--repo $(HELMREPO) \
	--version $(VERSION) \
	--release-name $(RELEASE) \
	$(CHART)
