

- PackageDescription
-  SwiftSetting 

Structure

# SwiftSetting

A Swift language build setting.

``` source
struct SwiftSetting
```

## Topics

### Configuring Swift Settings

static func define(String, BuildSettingCondition?) -> SwiftSetting

Defines a compilation condition.

static func unsafeFlags([String], BuildSettingCondition?) -> SwiftSetting

Set unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

### Type Methods

static func enableExperimentalFeature(String, BuildSettingCondition?) -> SwiftSetting

Enable an experimental feature with the given name.

static func enableUpcomingFeature(String, BuildSettingCondition?) -> SwiftSetting

Enable an upcoming feature with the given name.

static func interoperabilityMode(SwiftSetting.InteroperabilityMode, BuildSettingCondition?) -> SwiftSetting

Enable Swift interoperability with a given language.

static func swiftLanguageMode(SwiftLanguageMode, BuildSettingCondition?) -> SwiftSetting

Defines a `-language-mode` to pass to the corresponding build tool.

static func swiftLanguageVersion(SwiftVersion, BuildSettingCondition?) -> SwiftSetting

Defines a `-swift-version` to pass to the corresponding build tool.

Deprecated

### Enumerations

enum InteroperabilityMode

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

struct LinkerSetting

A linker build setting.

enum PluginUsage

A plug-in used in a target.

