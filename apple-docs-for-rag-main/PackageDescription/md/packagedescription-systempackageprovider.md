

- PackageDescription
-  SystemPackageProvider 

Enumeration

# SystemPackageProvider

The system package providers that this package uses.

``` source
enum SystemPackageProvider
```

## Topics

### Providing Hints to Users of System Packages

static func brew([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for people who use the HomeBrew package manager on macOS.

static func apt([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the apt-get package manager on Ubuntu Linux.

static func yum([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the yum package manager on Red Hat Enterprise Linux or CentOS.

### Enumeration Cases

case aptItem([String])

Packages installable by the apt-get package manager.

case brewItem([String])

Packages installable by the HomeBrew package manager.

case nugetItem([String])

Packages installable by the NuGet package manager.

case yumItem([String])

Packages installable by the Yellowdog Updated, Modified (YUM) package manager.

### Type Methods

static func nuget([String]) -> SystemPackageProvider

Creates a system package provider with a list of installable packages for users of the NuGet package manager on Linux or Windows.

## See Also

### Configuring System Packages

var pkgConfig: String?

The name to use for C modules.

var providers: [SystemPackageProvider]?

An array of providers for a system target.

