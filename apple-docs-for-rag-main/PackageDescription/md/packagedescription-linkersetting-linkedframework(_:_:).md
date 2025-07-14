

- PackageDescription
- LinkerSetting
-  linkedFramework(\_:\_:) 

Type Method

# linkedFramework(\_:\_:)

Declares linkage to a system framework.

SwiftPM 5.0+

``` source
static func linkedFramework(
    _ framework: String,
    _ condition: BuildSettingCondition? = nil
) -> LinkerSetting
```

## Parameters 

`framework`  

The framework name.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

This setting is most useful when the framework can’t be linked automatically, such as C++ based frameworks and non-modular frameworks.

Since

First available in PackageDescription 5.0.

## See Also

### Configuring Linker Settings

static func linkedLibrary(String, BuildSettingCondition?) -> LinkerSetting

Declares linkage to a system library.

static func unsafeFlags([String], BuildSettingCondition?) -> LinkerSetting

Sets unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

