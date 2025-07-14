

- PackageDescription
-  LinkerSetting 

Structure

# LinkerSetting

A linker build setting.

``` source
struct LinkerSetting
```

## Topics

### Configuring Linker Settings

static func linkedFramework(String, BuildSettingCondition?) -> LinkerSetting

Declares linkage to a system framework.

static func linkedLibrary(String, BuildSettingCondition?) -> LinkerSetting

Declares linkage to a system library.

static func unsafeFlags([String], BuildSettingCondition?) -> LinkerSetting

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

struct CXXSetting

A CXX-language build setting.

struct SwiftSetting

A Swift language build setting.

enum PluginUsage

A plug-in used in a target.

