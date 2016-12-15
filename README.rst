cookiecutter-docker
===================

cookiecutter template for docker based projects


Features
--------

- Boilerplate for `Alpine <https://alpinelinux.org/>`_ or `Debian <https://debian.org>`_ based Dockerfiles.
- Setup of project structure including documenation, changes and license.
- Setup of custom *Makefile* for building, taging and pushing images [currently `docker-hub <https://hub.docker.com/>`_ and `Quay <https://quay.io/>`_].


Examples
--------

.. raw:: html

	<a href="https://asciinema.org/a/8e4bhblj5xcpqqtzn80qn7er2" target="_blank"><img src="https://asciinema.org/a/8e4bhblj5xcpqqtzn80qn7er2.png" width="835"></a>


Usage
-----

Make sure that you have `cookiecutter <https://github.com/audreyr/cookiecutter>`_ installed.

Now run it against this repo:

.. code-block:: shell

	cookiecutter https://github.com/svx/cookiecutter-docker


.. code-block:: shell

	project_name [projectx]: my-cool-project
	Select docker_base:
	1 - alpine:latest
	2 - debian:jessie
	Choose from 1, 2 [1]: 1
	maintainer_name [Sven]: 
	maintainer_mail [sven@so36.net]: 
	short_description [A short description which will be used in the README]: This is so awesome
	repo_group [User or Orga name on GitHub]: svx
	repo_name [my-cool-project]: 
	docker_repo [User or Orga name for registry]: svx
	Select docker_registry:
	1 - quay.io
	2 - docker-hub
	Choose from 1, 2 [1]: 1
	version_nr [0.1]: 
	Select open_source_license:
	1 - MIT license
	2 - BSD license
	3 - ISC license
	4 - Apache Software License 2.0
	5 - GNU General Public License v3
	6 - Not open source
	Choose from 1, 2, 3, 4, 5, 6 [1]: 5



Support
-------

If you are having issues, please let us know.


