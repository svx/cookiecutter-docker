FROM {{cookiecutter.docker_base}}
MAINTAINER {{cookiecutter.maintainer_name}} <{{cookiecutter.maintainer_mail}}>

{% if cookiecutter.docker_base == 'alpine:latest' %}
LABEL os="alpine" os.version="3.4"

RUN apk --no-cache add \

{% elif cookiecutter.docker_base == 'debian:jessie' %}
LABEL os="debian" os.version="8"

RUN apt-get update && apt-get install -y \
{% endif %}

VOLUME

WORKDIR

ADD

EXPOSE


# Make sure to check if tini [https://github.com/krallin/tini] could be useful
ENTRYPOINT

CMD
