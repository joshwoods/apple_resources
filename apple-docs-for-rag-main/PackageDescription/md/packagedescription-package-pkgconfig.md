

- PackageDescription
- Package
-  pkgConfig 

Instance Property

# pkgConfig

The name to use for C modules.

``` source
final var pkgConfig: String?
```

## Discussion

If present, the Swift Package Manager searches for a `.pc` file to get the required additional flags for a system target.

## See Also

### Configuring System Packages

enum SystemPackageProvider

The system package providers that this package uses.

var providers: [SystemPackageProvider]?

An array of providers for a system target.

