

- PackageDescription
- Target
-  pkgConfig 

Instance Property

# pkgConfig

The name of the package configuration file, without extension, for the system library target.

``` source
final let pkgConfig: String?
```

## Discussion

If present, the Swift Package Manager tries every package configuration name separated by a space to search for the `.pc` file to get the additional flags needed for the system library target.

## See Also

### Creating a System Target

static func systemLibrary(name: String, path: String?, pkgConfig: String?, providers: [SystemPackageProvider]?) -> Target

Creates a system library target.

let providers: [SystemPackageProvider]?

The providers array for a system library target.

