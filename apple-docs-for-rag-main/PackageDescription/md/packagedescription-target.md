

- PackageDescription
-  Target 

Class

# Target

The basic building block of a Swift package.

``` source
final class Target
```

## Overview

Each target contains a set of source files that Swift Package Manager compiles into a module or test suite. You can vend targets to other packages by defining products that include the targets.

A target may depend on other targets within the same package and on products vended by the package’s dependencies.

## Topics

### Naming the Target

var name: String

The name of the target.

### Configuring File Locations

var path: String?

The path of the target, relative to the package root.

var exclude: [String]

The paths to source and resource files that you don’t want to include in the target.

var sources: [String]?

The source files in this target.

var resources: [Resource]?

The explicit list of resource files in the target.

struct Resource

A resource to bundle with the Swift package.

var publicHeadersPath: String?

The path to the directory that contains public headers of a C-family target.

### Creating a Binary Target

static func binaryTarget(name: String, path: String) -> Target

Creates a binary target that references an artifact on disk.

static func binaryTarget(name: String, url: String, checksum: String) -> Target

Creates a binary target that references a remote artifact.

var url: String?

The URL of a binary target.

var checksum: String?

The checksum for the archive file that contains the referenced binary artifact.

### Creating a System Target

static func systemLibrary(name: String, path: String?, pkgConfig: String?, providers: [SystemPackageProvider]?) -> Target

Creates a system library target.

let pkgConfig: String?

The name of the package configuration file, without extension, for the system library target.

let providers: [SystemPackageProvider]?

The providers array for a system library target.

### Creating an Executable Target

static func executableTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, publicHeadersPath: String?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?) -> Target

Creates an executable target.

Deprecated

static func executableTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, publicHeadersPath: String?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

Creates an executable target.

Deprecated

### Creating a Plugin Target

static func plugin(name: String, capability: Target.PluginCapability, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?) -> Target

Defines a new package plugin target.

Deprecated

var pluginCapability: Target.PluginCapability?

The capability provided by a package plug-in target.

enum PluginCapability

The different types of capability that a plug-in can provide.

enum PluginCommandIntent

The intended use case of the command plug-in.

enum PluginPermission

The type of permission a plug-in requires.

### Declaring a Dependency Target

var dependencies: [Target.Dependency]

The target’s dependencies on other entities inside or outside the package.

enum Dependency

The different types of a target’s dependency on another entity.

struct TargetDependencyCondition

A condition that limits the application of a target’s dependency.

### Configuring the Target

var cSettings: [CSetting]?

The target’s C build settings.

var cxxSettings: [CXXSetting]?

The target’s C++ build settings.

var swiftSettings: [SwiftSetting]?

The target’s Swift build settings.

var linkerSettings: [LinkerSetting]?

The target’s linker settings.

var plugins: [Target.PluginUsage]?

The uses of package plug-ins by the target.

struct BuildConfiguration

The build configuration, such as debug or release.

struct BuildSettingCondition

A condition that limits the application of a build setting.

struct CSetting

A C language build setting.

struct CXXSetting

A CXX-language build setting.

struct SwiftSetting

A Swift language build setting.

struct LinkerSetting

A linker build setting.

enum PluginUsage

A plug-in used in a target.

### Describing the Target Type

var isTest: Bool

A Boolean value that indicates whether this is a test target.

let type: Target.TargetType

The type of the target.

enum TargetType

The different types of a target.

### Instance Properties

let packageAccess: Bool

If true, access to package declarations from other targets in the package is allowed.

### Type Methods

static func executableTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, publicHeadersPath: String?, packageAccess: Bool, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

Creates an executable target.

static func macro(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, packageAccess: Bool, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

static func plugin(name: String, capability: Target.PluginCapability, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, packageAccess: Bool) -> Target

Defines a new package plug-in target.

static func target(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, publicHeadersPath: String?) -> Target

Creates a library or executable target.

Deprecated

static func target(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, publicHeadersPath: String?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?) -> Target

Creates a library or executable target.

Deprecated

static func target(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, publicHeadersPath: String?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?) -> Target

Creates a regular target.

Deprecated

static func target(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, publicHeadersPath: String?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

Creates a regular target.

Deprecated

static func target(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, publicHeadersPath: String?, packageAccess: Bool, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

Creates a regular target.

static func testTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?) -> Target

Creates a test target.

Deprecated

static func testTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?) -> Target

Creates a test target.

Deprecated

static func testTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?) -> Target

Creates a test target.

Deprecated

static func testTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

Creates a test target.

Deprecated

static func testTarget(name: String, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?, resources: [Resource]?, packageAccess: Bool, cSettings: [CSetting]?, cxxSettings: [CXXSetting]?, swiftSettings: [SwiftSetting]?, linkerSettings: [LinkerSetting]?, plugins: [Target.PluginUsage]?) -> Target

Creates a test target.

## See Also

### Configuring Targets

var targets: [Target]

The list of targets that are part of this package.

