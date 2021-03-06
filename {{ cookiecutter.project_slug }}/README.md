# {{ cookiecutter.project_name }}

## Overview

{{ cookiecutter.project_overview }}

## Required Dependencies

* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)

## Optional Dependencies

* [Yarn](https://yarnpkg.com/en/)
* [Cygwin](https://www.cygwin.com) if you're using Windows. This will allow you
  to use the helper scripts such as `ssh_frontend.sh`.
* An X11 server such as [XQuartz](https://www.xquartz.org) for Mac or
  [Cygwin/X](https://x.cygwin.com) for Windows.

## Quickstart

To provision the development environment, run:
```
$ cd {{ cookiecutter.project_slug }}
$ vagrant up --provision
```

You may need to re-run this command if Vagrant needed to install plugins.
You may also be prompted for a password if the `vagrant-vbguest` plugin is
making changes to your `/etc/hosts` file.

Once provisioning has finished, you can access the django app at https://{{ cookiecutter.backend_app_dev_hostname }}
and the frontend app at https://{{ cookiecutter.frontend_app_dev_hostname }}

## Next Steps

Read the following documentation for more information:

* [Backend App](docs/backend_app.md)
* [Frontend App](docs/frontend_app.md)
* [Provisioning](docs/provisioning.md)
* [Other Tools](docs/other_tools.md)
* [Configuring PyCharm](docs/configuring_pycharm.md)
