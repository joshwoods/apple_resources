

- PackageDescription
- Package
-  init(name:defaultLocalization:platforms:pkgConfig:providers:products:dependencies:targets:swiftLanguageVersions:cLanguageStandard:cxxLanguageStandard:) Deprecated

Initializer

# init(name:defaultLocalization:platforms:pkgConfig:providers:products:dependencies:targets:swiftLanguageVersions:cLanguageStandard:cxxLanguageStandard:)

Initializes a Swift package with configuration options you provide.

SwiftPM 5.3–6.0Deprecated

``` source
init(
    name: String,
    defaultLocalization: LanguageTag? = nil,
    platforms: [SupportedPlatform]? = nil,
    pkgConfig: String? = nil,
    providers: [SystemPackageProvider]? = nil,
    products: [Product] = [],
    dependencies: [Package.Dependency] = [],
    targets: [Target] = [],
    swiftLanguageVersions: [SwiftVersion]? = nil,
    cLanguageStandard: CLanguageStandard? = nil,
    cxxLanguageStandard: CXXLanguageStandard? = nil
)
```

## Parameters 

`name`  

The name of the Swift package, or `nil` to use the package’s Git URL to deduce the name.

`defaultLocalization`  

The default localization for resources.

`platforms`  

The list of supported platforms with a custom deployment target.

`pkgConfig`  

The name to use for C modules. If present, Swift Package Manager searches for a `.pc` file to get the additional flags required for a system target.

`providers`  

The package providers for a system target.

`products`  

The list of products that this package makes available for clients to use.

`dependencies`  

The list of package dependencies.

`targets`  

The list of targets that are part of this package.

`swiftLanguageVersions`  

The list of Swift versions with which this package is compatible.

`cLanguageStandard`  

The C language standard to use for all C targets in this package.

`cxxLanguageStandard`  

The C++ language standard to use for all C++ targets in this package.

