

- PackageDescription
- Target
-  providers 

Instance Property

# providers

The providers array for a system library target.

``` source
final let providers: [SystemPackageProvider]?
```

## See Also

### Creating a System Target

static func systemLibrary(name: String, path: String?, pkgConfig: String?, providers: [SystemPackageProvider]?) -> Target

Creates a system library target.

let pkgConfig: String?

The name of the package configuration file, without extension, for the system library target.

