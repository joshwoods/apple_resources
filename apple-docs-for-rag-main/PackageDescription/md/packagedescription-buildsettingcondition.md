

- PackageDescription
-  BuildSettingCondition 

Structure

# BuildSettingCondition

A condition that limits the application of a build setting.

``` source
struct BuildSettingCondition
```

## Overview

By default, build settings are applicable for all platforms and build configurations. Use the `.when` modifier to define a build setting for a specific condition. Invalid usage of `.when` emits an error during manifest parsing. For example, it’s invalid to specify a `.when` condition with both parameters as `nil`.

The following example shows how to use build setting conditions with various APIs:

```
...
.target(
    name: "MyTool",
    dependencies: ["Utility"],
    cSettings: [
        .headerSearchPath("path/relative/to/my/target"),
        .define("DISABLE_SOMETHING", .when(platforms: [.iOS], configuration: .release)),
    ],
    swiftSettings: [
        .define("ENABLE_SOMETHING", .when(configuration: .release)),
    ],
    linkerSettings: [
        .linkLibrary("openssl", .when(platforms: [.linux])),
    ]
),
```

## Topics

### Checking for a Build Condition

static func when(platforms: [Platform]) -> BuildSettingCondition

Creates a build setting condition.

static func when(configuration: BuildConfiguration) -> BuildSettingCondition

Creates a build setting condition.

static func when(platforms: [Platform]?, configuration: BuildConfiguration?) -> BuildSettingCondition

Creates a build setting condition.

Deprecated

static func when(platforms: [Platform], configuration: BuildConfiguration) -> BuildSettingCondition

Creates a build setting condition.

### Type Methods

static func when(platforms: [Platform]?, configuration: BuildConfiguration?, traits: Set&lt;String>?) -> BuildSettingCondition

Creates a build setting condition.

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

