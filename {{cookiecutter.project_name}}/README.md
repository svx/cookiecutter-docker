# {{cookiecutter.project_name}}


{{cookiecutter.short_description}}

## Features


## Documentation


Full documentation for end users can be found in the "docs" folder.

## Installation


## Contribute


* [Issue Tracker](https://github.com/{{cookiecutter.repo_group}}/{{cookiecutter.repo_name}}/issues)
* [Source Code](https://github.com/{{cookiecutter.repo_group}}/{{cookiecutter.repo_name}})

## License

{% if cookiecutter.open_source_license == 'MIT license' %}
MIT License
{% elif cookiecutter.open_source_license == 'BSD license' %}
BSD License
{% elif cookiecutter.open_source_license == 'ISC license' %}
ISC License
{% elif cookiecutter.open_source_license == 'Apache Software License 2.0' %}
Apache Software License 2.0
{% elif cookiecutter.open_source_license == 'GNU General Public License v3' %}
GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
{% endif %}
