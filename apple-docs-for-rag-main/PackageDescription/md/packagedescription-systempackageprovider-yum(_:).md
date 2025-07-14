

- PackageDescription
- SystemPackageProvider
-  yum(\_:) 

Type Method

# yum(\_:)

Creates a system package provider with a list of installable packages for users of the yum package manager on Red Hat Enterprise Linux or CentOS.

SwiftPM 5.3+

``` source
static func yum(_ packages: [String]) -> SystemPackageProvider
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

static func apt([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the apt-get package manager on Ubuntu Linux.

