
IMAGE_PREFIX ?= envoyproxy/gateway-
APP_NAME ?= envoy-ext-auth
TAG ?= latest
GO_LDFLAGS ?=
BUILDX_EXTRA_ARGS ?=

.PHONY: docker-buildx
docker-buildx:
	docker buildx build . -t $(IMAGE_PREFIX)$(APP_NAME):$(TAG) --build-arg GO_LDFLAGS="$(GO_LDFLAGS)" $(BUILDX_EXTRA_ARGS) --load
