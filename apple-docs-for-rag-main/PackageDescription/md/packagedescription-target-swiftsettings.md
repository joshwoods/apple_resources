

- PackageDescription
- Target
-  swiftSettings 

Instance Property

# swiftSettings

The target’s Swift build settings.

SwiftPM 5.0+

``` source
final var swiftSettings: [SwiftSetting]?
```

## See Also

### Configuring the Target

var cSettings: [CSetting]?

The target’s C build settings.

var cxxSettings: [CXXSetting]?

The target’s C++ build settings.

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

