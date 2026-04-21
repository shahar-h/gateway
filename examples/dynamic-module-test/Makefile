
IMAGE_PREFIX ?= envoyproxy/gateway-
APP_NAME ?= dynamic-module-test
TAG ?= latest
ENVOY_VERSION ?= dev
BUILDX_EXTRA_ARGS ?=

.PHONY: docker-buildx
docker-buildx:
	docker buildx build . --build-arg ENVOY_VERSION=$(ENVOY_VERSION) -t $(IMAGE_PREFIX)$(APP_NAME):$(TAG) $(BUILDX_EXTRA_ARGS) --load
