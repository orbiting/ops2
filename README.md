# ops2

We currently host all of our production systems on heroku, with some exception, which we run on [exoscale](exoscale.ch) and which are maintained through this repo.

This repo is the successor of the obsolete [ops](https://github.com/orbiting/ops) repo and contains the remaining active parts.


## Set up your sysadmin machine

### install CLI tools
To interact with our deployments you need to have the following tools installed.
- SSH client (duh!)
- [ansible](http://docs.ansible.com/ansible/intro_installation.html)
- [docker](https://docs.docker.com/engine/installation/)
- [docker-compose](https://docs.docker.com/compose/install/)
- [docker-machine](https://docs.docker.com/machine/install-machine/)
- [gopass](https://www.justwatch.com/gopass/) / [pass](https://www.passwordstore.org/)

## Secrets
We manage our passwords and keys with [gopass](https://github.com/justwatchcom/gopass). Checkout the repository like this
```
gopass clone https://git.project-r.construction/admins/pass r  # clone as mount called: r
```
