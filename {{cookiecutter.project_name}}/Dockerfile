FROM {{cookiecutter.docker_base}}
MAINTAINER {{cookiecutter.maintainer_name}} <{{cookiecutter.maintainer_mail}}>

{% if cookiecutter.docker_base == 'alpine:latest' %}
RUN apk --no-cache add \

{% elif cookiecutter.docker_base == 'debian:jessie' %}
RUN apt-get update && apt-get install -y \
{% endif %}
