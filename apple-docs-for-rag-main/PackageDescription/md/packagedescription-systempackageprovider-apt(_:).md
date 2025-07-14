

- PackageDescription
- SystemPackageProvider
-  apt(\_:) 

Type Method

# apt(\_:)

Creates a system package provider with a list of installable packages for users of the apt-get package manager on Ubuntu Linux.

``` source
static func apt(_ packages: [String]) -> SystemPackageProvider
```

## Parameters 

`packages`  

The list of package names.

## Return Value

A package provider.

## See Also

### Providing Hints to Users of System Packages

static func brew([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for people who use the HomeBrew package manager on macOS.

static func yum([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the yum package manager on Red Hat Enterprise Linux or CentOS.

