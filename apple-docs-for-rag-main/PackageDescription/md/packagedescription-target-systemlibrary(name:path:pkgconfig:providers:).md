

- PackageDescription
- Target
-  systemLibrary(name:path:pkgConfig:providers:) 

Type Method

# systemLibrary(name:path:pkgConfig:providers:)

Creates a system library target.

``` source
static func systemLibrary(
    name: String,
    path: String? = nil,
    pkgConfig: String? = nil,
    providers: [SystemPackageProvider]? = nil
) -> Target
```

## Parameters 

`name`  

The name of the target.

`path`  

The custom path for the target. By default, a targets sources are expected to be located in the predefined search paths, such as `[PackageRoot]/Sources/[TargetName]`. Do not escape the package root; that is, values like `../Foo` or `/Foo` are invalid.

`pkgConfig`  

The name of the `pkg-config` file for this system library.

`providers`  

The providers for this system library.

## Discussion

Use system library targets to adapt a library installed on the system to work with Swift packages. Such libraries are generally installed by system package managers (such as Homebrew and apt-get) and exposed to Swift packages by providing a `modulemap` file along with other metadata such as the library’s `pkgConfig` name.

## See Also

### Creating a System Target

let pkgConfig: String?

The name of the package configuration file, without extension, for the system library target.

let providers: [SystemPackageProvider]?

The providers array for a system library target.

