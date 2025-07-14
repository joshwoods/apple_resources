

- PackageDescription
-  Package 

Class

# Package

The configuration of a Swift package.

``` source
final class Package
```

## Overview

Pass configuration options as parameters to your package’s initializer statement to provide the name of the package, its targets, products, dependencies, and other configuration options.

By convention, you need to define the properties of a package in a single nested initializer statement. Don’t modify it after initialization. The following package manifest shows the initialization of a simple package object for the MyLibrary Swift package:

```
// swift-tools-version:5.3
import PackageDescription

let package = Package(
    name: "MyLibrary",
    platforms: [
        .macOS(.v10_15),
    ],
    products: [
        .library(name: "MyLibrary", targets: ["MyLibrary"])
    ],
    dependencies: [
        .package(url: "https://url/of/another/package/named/utility", from: "1.0.0")
    ],
    targets: [
        .target(name: "MyLibrary", dependencies: ["Utility"]),
        .testTarget(name: "MyLibraryTests", dependencies: ["MyLibrary"])
    ]
)
```

In Swift tools versions earlier than 5.4, the package manifest must begin with the string `// swift-tools-version:` followed by a version number specifier. Version 5.4 and later has relaxed the whitespace requirements. The following code listing shows a few examples of valid declarations of the Swift tools version:

```
// swift-tools-version:3.0.2
// swift-tools-version:3.1
// swift-tools-version:4.0
// swift-tools-version:5.3
// swift-tools-version: 5.6
```

The Swift tools version declares the version of the `PackageDescription` library, the minimum version of the Swift tools and Swift language compatibility version to process the manifest, and the required minimum version of the Swift tools to use the Swift package. Each version of Swift can introduce updates to the PackageDescription framework, but the previous API version is available to packages which declare a prior tools version. This behavior means you can take advantage of new releases of Swift, the Swift tools, and the PackageDescription library, without having to update your package’s manifest or losing access to existing packages.

## Topics

### Creating a Package

init(name: String, defaultLocalization: LanguageTag?, platforms: [SupportedPlatform]?, pkgConfig: String?, providers: [SystemPackageProvider]?, products: [Product], dependencies: [Package.Dependency], targets: [Target], swiftLanguageVersions: [SwiftVersion]?, cLanguageStandard: CLanguageStandard?, cxxLanguageStandard: CXXLanguageStandard?)

Initializes a Swift package with configuration options you provide.

Deprecated

### Naming the Package

var name: String

The name of the Swift package.

### Localizing Package Resources

var defaultLocalization: LanguageTag?

The default localization for resources.

struct LanguageTag

A wrapper around an IETF language tag.

### Configuring Products

var products: [Product]

The list of products that this package vends and that clients can use.

class Product

The object that defines a package product.

### Configuring Targets

var targets: [Target]

The list of targets that are part of this package.

class Target

The basic building block of a Swift package.

### Declaring Supported Platforms

var platforms: [SupportedPlatform]?

The list of minimum versions for platforms supported by the package.

struct SupportedPlatform

A platform that the Swift package supports.

struct Platform

A platform supported by Swift Package Manager.

### Configuring System Packages

enum SystemPackageProvider

The system package providers that this package uses.

var pkgConfig: String?

The name to use for C modules.

var providers: [SystemPackageProvider]?

An array of providers for a system target.

### Declaring Package Dependencies

var dependencies: [Package.Dependency]

The list of package dependencies.

class Dependency

A package dependency of a Swift package.

### Declaring Supported Languages

typealias SwiftVersion

Type alias to previous name for backward source compatibility

Deprecated

enum CLanguageStandard

The supported C language standard you use to compile C sources in the package.

enum CXXLanguageStandard

The supported C++ language standard you use to compile C++ sources in the package.

var swiftLanguageVersions: [SwiftVersion]?

Legacy property name, accesses value of `swiftLanguageModes`

Deprecated

var cLanguageStandard: CLanguageStandard?

The C language standard to use for all C targets in this package.

var cxxLanguageStandard: CXXLanguageStandard?

The C++ language standard to use for all C++ targets in this package.

### Initializers

init(name: String, defaultLocalization: LanguageTag?, platforms: [SupportedPlatform]?, pkgConfig: String?, providers: [SystemPackageProvider]?, products: [Product], dependencies: [Package.Dependency], targets: [Target], swiftLanguageModes: [SwiftLanguageMode]?, cLanguageStandard: CLanguageStandard?, cxxLanguageStandard: CXXLanguageStandard?)

Initializes a Swift package with configuration options you provide.

init(name: String, defaultLocalization: LanguageTag?, platforms: [SupportedPlatform]?, pkgConfig: String?, providers: [SystemPackageProvider]?, products: [Product], traits: Set&lt;Trait>, dependencies: [Package.Dependency], targets: [Target], swiftLanguageModes: [SwiftLanguageMode]?, cLanguageStandard: CLanguageStandard?, cxxLanguageStandard: CXXLanguageStandard?)

Initializes a Swift package with configuration options you provide.

init(name: String, pkgConfig: String?, providers: [SystemPackageProvider]?, products: [Product], dependencies: [Package.Dependency], targets: [Target], swiftLanguageVersions: [SwiftVersion]?, cLanguageStandard: CLanguageStandard?, cxxLanguageStandard: CXXLanguageStandard?)

Initializes a Swift package with configuration options you provide.

Deprecated

init(name: String, pkgConfig: String?, providers: [SystemPackageProvider]?, products: [Product], dependencies: [Package.Dependency], targets: [Target], swiftLanguageVersions: [Int]?, cLanguageStandard: CLanguageStandard?, cxxLanguageStandard: CXXLanguageStandard?)

Initializes a Swift package with configuration options you provide.

Deprecated

init(name: String, platforms: [SupportedPlatform]?, pkgConfig: String?, providers: [SystemPackageProvider]?, products: [Product], dependencies: [Package.Dependency], targets: [Target], swiftLanguageVersions: [SwiftVersion]?, cLanguageStandard: CLanguageStandard?, cxxLanguageStandard: CXXLanguageStandard?)

Initializes a Swift package with configuration options you provide.

Deprecated

### Instance Properties

var swiftLanguageModes: [SwiftLanguageMode]?

The list of Swift language modes with which this package is compatible.

var traits: Set&lt;Trait>

The set of traits of this package.

## See Also

### Creating a Package

struct Context

The context information for a Swift package.

