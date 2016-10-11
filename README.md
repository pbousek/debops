## [![DebOps](https://debops.org/images/debops-small.png)](https://debops.org) owncloud

<!-- This file was generated by Ansigenome. Do not edit this file directly but
     instead have a look at the files in the ./meta/ directory. -->

[![Travis CI](https://img.shields.io/travis/debops/ansible-owncloud.svg?style=flat)](https://travis-ci.org/debops/ansible-owncloud)
[![test-suite](https://img.shields.io/badge/test--suite-ansible--owncloud-blue.svg?style=flat)](https://github.com/debops/test-suite/tree/master/ansible-owncloud/)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-debops.owncloud-660198.svg?style=flat)](https://galaxy.ansible.com/debops/owncloud)


This role installs a [ownCloud](https://owncloud.org/) instance on a
specified host, either with SQLite, MySQL, MariaDB or PostgreSQL database
as a backend and an nginx webserver as a frontend.

Only ownCloud 8.0 and later are supported because for older
versions there are no complete deb-packages available.

Note that Nginx is
[not officially supported by ownCloud nor NextCloud](https://github.com/debops/ansible-owncloud/issues/49)
but it is community supported and should work without problems.
Apache is supported by the role but not yet used by default.

### Features

* LDAP setup.
* In memory caching using Redis for file locking and APCu.
* Fully automated ownCloud security updates.
* ownCloud theming support.
* Extensive configuration options via Ansible’s inventory.
* Fully automated ownCloud security updates. [Not yet enabled by default](https://github.com/debops/ansible-owncloud/issues/28).

### Installation

This role requires at least Ansible `v2.1.0`. To install it, run:

```Shell
ansible-galaxy install debops.owncloud
```

### Documentation

More information about `debops.owncloud` can be found in the
[official debops.owncloud documentation](https://docs.debops.org/en/latest/ansible/roles/ansible-owncloud/docs/).


### Role dependencies

- `debops.secret`

### Are you using this as a standalone role without DebOps?

You may need to include missing roles from the [DebOps common
playbook](https://github.com/debops/debops-playbooks/blob/master/playbooks/common.yml)
into your playbook.

[Try DebOps now](https://debops.org/) for a complete solution to run your Debian-based infrastructure.





### Authors and license

- [Maciej Delmanowski](https://docs.debops.org/en/latest/debops-keyring/docs/entities.html#debops-keyring-entity-drybjed) | [e-mail](mailto:drybjed@gmail.com) | [Twitter](https://twitter.com/drybjed) | [GitHub](https://github.com/drybjed)
- [Robin Schneider](https://docs.debops.org/en/latest/debops-keyring/docs/entities.html#debops-keyring-entity-ypid) (maintainer) | [e-mail](mailto:ypid@riseup.net) | [GitHub](https://github.com/ypid)
- [Hartmut Goebel](http://www.crazy-compilers.com/) | [e-mail](mailto:h.goebel@crazy-compilers.com) | [GitHub](https://github.com/htgoebel)

License: [GPL-3.0](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

***

This role is part of the [DebOps](https://debops.org/) project. README generated by [ansigenome](https://github.com/nickjj/ansigenome/).
