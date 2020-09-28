[![Build Status](https://dev.azure.com/chefcorp-partnerengineering/Chef%20Base%20Plans/_apis/build/status/chef-base-plans.nss-myhostname?branchName=master)](https://dev.azure.com/chefcorp-partnerengineering/Chef%20Base%20Plans/_build/latest?definitionId=274&branchName=master)

# nss-myhostname

nss-myhostname is a plugin for the GNU Name Service Switch (NSS) functionality of the GNU C Library (glibc) providing host name resolution for the locally configured system hostname as returned by gethostname(2). This plugin is commonly enabled in the default `/etc/nsswitch.conf` NSS configuration of RHEL and RHEL-like Linux distributions. glibc has `/etc/nsswitch.conf` hard-coded as the file location for configuration. So long as core/glibc ships with that setting, this plugin is necessary for some software to perform name resolution with expected behavior.  See [documentation](http://0pointer.de/lennart/projects/nss-myhostname/) 

## Maintainers

* The Core Planners: <chef-core-planners@chef.io>

## Type of Package

Binary package

### Use as Dependency

Binary packages can be set as runtime or build time dependencies. See [Defining your dependencies](https://www.habitat.sh/docs/developing-packages/developing-packages/#sts=Define%20Your%20Dependencies) for more information.

To add core/nss-myhostname as a dependency, you can add one of the following to your plan file.

#### Buildtime Dependency

> pkg_build_deps=(core/nss-myhostname)

#### Runtime dependency

> pkg_deps=(core/nss-myhostname)

### Use as Tool

#### Installation

To install this plan, you should run the following commands to first install, and then link the binaries this plan creates.

``hab pkg install core/nss-myhostname --binlink``

will add the following binaries to the PATH:

* TODO - Copy the binlink output and then run ``bins``
* TODO - Add binary
* TODO - Add binary

For example:

```bash
$ hab pkg install core/nss-myhostname --binlink
TODO: ADD THE OUTPUT HERE
```

##### Additional Steps

TODO: ADD OR DELETE THIS SECTION AS NEEDED 

To use core/nss-myhostname as a stand alone binary, you must configure ...

#### Using an example binary

You can now use the binary as normal.  For example:

``/bin/nss-myhostname --help`` or ``nss-myhostname --help``

```bash
$ nss-myhostname --help
TODO:  ADD SOME OUTPUT HERE, BUT NO MORE THAN 10-15 lines...
```
