Build environment for building RHEL Distribution packages

Works for CentOS8 and CentOS9.
Tested in Oracle Linux 8, 9


Make will fetch the version from GitHub.

E.g. You can build a devel repo like this:

    VERSION=3.8.1 make clean buildrpm 

If you want to build privacyidea-selinux you need to adapt the privacyidea-selinux.spec file and run:

    make clean buildselinux fill-release-repo make-repo push-repo

