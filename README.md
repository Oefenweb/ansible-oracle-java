## oracle-java

[![Build Status](https://travis-ci.org/Oefenweb/ansible-oracle-java.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-oracle-java) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-oracle--java-blue.svg)](https://galaxy.ansible.com/list#/roles/1854)

Set up any version of  oracle-java in Ubuntu systems.



#### Requirements

* `python-apt`
* `update-alternatives`

#### Variables

* `oracle_java_versions`
  [default: `[{version: 7, set_as_default: true,update_version}]`]: Oracle java  version(s) to install, whether or not to set as default and (optionally) the  java update version to use.
  
  The java update version must be the version of webupd8team (see https://launchpad.net/~webupd8team/+archive/ubuntu/java for a list of all versions). If the variable is not used, the latest update version is installed
  
  

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
