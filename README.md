## oracle-java

[![Build Status](https://travis-ci.org/Oefenweb/ansible-oracle-java.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-oracle-java) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-oracle-java-blue.svg)](https://galaxy.ansible.com/list#/roles/1854)

Set up (the latest version of) oracle-java in Ubuntu systems.

#### Requirements

* `python-apt`
* `update-alternatives`

#### Variables

* `oracle_java_versions` [default: `[{version: 7, set_as_default: true}]`]: Oracle java version(s) to install and whether or not to set as default

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - oracle-java
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-oracle-java/issues)!
