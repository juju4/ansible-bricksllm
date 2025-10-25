[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
# DEPRECATED/LOOKING FOR MAINTAINERS -> to be archived soon

[![Actions Status - Master](https://github.com/juju4/ansible-bricksllm/workflows/AnsibleCI/badge.svg)](https://github.com/juju4/ansible-bricksllm/actions?query=branch%3Amaster)
[![Actions Status - Devel](https://github.com/juju4/ansible-bricksllm/workflows/AnsibleCI/badge.svg?branch=devel)](https://github.com/juju4/ansible-bricksllm/actions?query=branch%3Adevel)

# BricksLLM ansible role

Ansible role to setup [BricksLLM, Enterprise-grade API gateway that helps you monitor and impose cost or rate limits per API key](https://github.com/bricks-cloud/BricksLLM)

Alternatives
* [LiteLLM Proxy Server](https://docs.litellm.ai/docs/simple_proxy), https://github.com/BerriAI/litellm, https://docs.litellm.ai/docs/proxy/enterprise
* https://observeapi.ashishb.net/

## Requirements & Dependencies

### Ansible
It was tested on the following versions:
 * 2.17

### Operating systems

Tested on Ubuntu 24.04, 22.04, Centos/Rockylinux 9, Debian 12 and 11.

## Example Playbook

Just include this role in your list.
For example

```
- host: myhost
  roles:
    - juju4.bricksllm
```

you probably want to review variables

## Variables

N/A

## Continuous integration

```
$ pip install molecule docker
$ molecule test
$ MOLECULE_DISTRO=ubuntu:24.04 molecule test --destroy=never
```

## Troubleshooting & Known issues

TBD

## License

BSD 2-clause
