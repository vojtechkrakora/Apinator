# Apinator
Ansible orchestration for WSO2 APIM - to manage APIs

## About
Because not everybody likes 'GUI development' this *Ansible* project adds possibility to
to automatize and version `WSO2-APIM` apis, scopes etc.

## Requirements
Ansible in version 2.9.6.

## Operations

:warning: **All operations are very naive now. They are using Jinja templates, but the templates does not
have varibles. So they are static and will allways create the same scope or API if not edited.** :warning:

All playbooks are now expecting, that WSO2 APIM is running on default ports on localhost.

### Create a shared scope
To create a shared scope in WSO2 APIM is playbook `createScope.yml`.

#### Command
`ansible-playbook createScope.yml`

### Create a new API
To create a new API in WSO2 APIM is playbook `createApi.yml`.

#### Command
`ansible-playbook createApi.yml`
