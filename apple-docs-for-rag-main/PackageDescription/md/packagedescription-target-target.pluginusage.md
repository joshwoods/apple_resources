

- PackageDescription
- Target
-  Target.PluginUsage 

Enumeration

# Target.PluginUsage

A plug-in used in a target.

SwiftPM 5.5+

``` source
enum PluginUsage
```

## Topics

### Creating a Plugin Usage

static func plugin(name: String) -> Target.PluginUsage

Specifies use of a plugin target in the same package.

case plugin(name: String, package: String?)

Specifies the use of a plug-in product in a package dependency.

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

## Relationships

### Conforms To

- Copyable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

## See Also

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

