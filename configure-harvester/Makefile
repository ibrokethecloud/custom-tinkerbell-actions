REGISTRY?=docker.io
REPOSITORY?=gmehta3/configure-harvester
VERSION?=latest
IMAGE=$(REGISTRY)/$(REPOSITORY):$(VERSION)

image:
	docker buildx build --load --platform linux/amd64 -t $(IMAGE) .

push: image
	docker push $(IMAGE)