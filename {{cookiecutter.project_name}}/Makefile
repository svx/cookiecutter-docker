# The shell we use
SHELL := /bin/bash

# We like colors
# From: https://coderwall.com/p/izxssa/colored-makefile-for-golang-projects
RED=`tput setaf 1`
GREEN=`tput setaf 2`
RESET=`tput sgr0`
YELLOW=`tput setaf 3`

# Name
NAME = {{cookiecutter.docker_repo}}/{{cookiecutter.project_name}}
# Get version form VERSION
VERSION := $(shell cat VERSION)

# Add the following 'help' target to your Makefile
# And add help text after each target name starting with '\#\#'
.PHONY: help
help: ## This help message
	@echo -e "$$(grep -hE '^\S+:.*##' $(MAKEFILE_LIST) | sed -e 's/:.*##\s*/:/' -e 's/^\(.\+\):\(.*\)/\\x1b[36m\1\\x1b[m:\2/' | column -c2 -t -s :)"

.PHONY: image
image: ## Builds docker image
	docker build -t $(NAME):$(VERSION) --rm .

.PHONY: push
push: ## Pushes images
{% if cookiecutter.docker_registry == 'docker-hub' %}
	docker push $(NAME):$(VERSION)

{% elif cookiecutter.docker_registry == 'quay.io' %}
	docker push quay.io/$(NAME):$(VERSION)
{% endif %}

.PHONY: tag_latest
tag_latest: ## Tag with version and latest tag
{% if cookiecutter.docker_registry == 'docker-hub' %}
	docker tag -f $(NAME):$(VERSION) $(NAME):latest

{% elif cookiecutter.docker_registry == 'quay.io' %}
	docker tag -f quay.io/$(NAME):$(VERSION) quay.io/$(NAME):latest

{% endif %}
