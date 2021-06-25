## oracle-java

[![Build Status](https://travis-ci.org/Oefenweb/ansible-oracle-java.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-oracle-java)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-oracle--java-blue.svg)](https://galaxy.ansible.com/Oefenweb/oracle_java)

Set up (the latest or a specific update version of) oracle-java in Ubuntu systems.

#### Requirements

* `update-alternatives`
* `software-properties-common` (will be installed)
* `dirmngr` (will be installed)

#### Variables

* `oracle_java_versions`: [default: `[{version: 7, set_as_default: true}]`]: Oracle java version(s) to install
* `oracle_java_versions.{n}.version`: [required]: Version to install
* `oracle_java_versions.{n}.set_as_default`: [optional]: Whether or not to set as default
* `oracle_java_versions.{n}.update_version`: [optional]: A specific update version to use (e.g. `8u121-1~webupd8~0`). Must be a version of [webupd8team](https://launchpad.net/~webupd8team/+archive/ubuntu/java). If undefined, the latest (update) version is installed

#### Dependencies

None

#### Example(s)

##### Simple

```yaml
---
- hosts: all
  roles:
    - oracle-java
```

##### Advanced

```yaml
---
- hosts: all
  roles:
    - oracle-java
  vars:
    oracle_java_versions:
      - version: 7
      - version: 8
        set_as_default: true
        update_version: '8u121-1~webupd8~0'
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-oracle-java/issues)!
