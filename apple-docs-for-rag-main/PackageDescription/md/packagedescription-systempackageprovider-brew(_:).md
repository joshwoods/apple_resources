

- PackageDescription
- SystemPackageProvider
-  brew(\_:) 

Type Method

# brew(\_:)

Creates a system package provider with a list of installable packages for people who use the HomeBrew package manager on macOS.

``` source
static func brew(_ packages: [String]) -> SystemPackageProvider
```

## Parameters 

`packages`  

The list of package names.

## Return Value

A package provider.

## See Also

### Providing Hints to Users of System Packages

static func apt([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the apt-get package manager on Ubuntu Linux.

static func yum([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the yum package manager on Red Hat Enterprise Linux or CentOS.

