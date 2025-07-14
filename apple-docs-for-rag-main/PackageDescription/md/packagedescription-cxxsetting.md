

- PackageDescription
-  CXXSetting 

Structure

# CXXSetting

A CXX-language build setting.

``` source
struct CXXSetting
```

## Topics

### Configuring CXX Settings

static func define(String, to: String?, BuildSettingCondition?) -> CXXSetting

Defines a value for a macro.

static func headerSearchPath(String, BuildSettingCondition?) -> CXXSetting

Provides a header search path relative to the target’s directory.

static func unsafeFlags([String], BuildSettingCondition?) -> CXXSetting

Sets unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

## Relationships

### Conforms To

- Sendable

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

struct SwiftSetting

A Swift language build setting.

struct LinkerSetting

A linker build setting.

enum PluginUsage

A plug-in used in a target.

