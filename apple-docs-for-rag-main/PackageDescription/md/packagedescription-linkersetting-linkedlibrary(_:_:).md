

- PackageDescription
- LinkerSetting
-  linkedLibrary(\_:\_:) 

Type Method

# linkedLibrary(\_:\_:)

Declares linkage to a system library.

SwiftPM 5.0+

``` source
static func linkedLibrary(
    _ library: String,
    _ condition: BuildSettingCondition? = nil
) -> LinkerSetting
```

## Parameters 

`library`  

The library name.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

This setting is most useful when the library can’t be linked automatically, such as C++ based libraries and non-modular libraries.

Since

First available in PackageDescription 5.0.

## See Also

### Configuring Linker Settings

static func linkedFramework(String, BuildSettingCondition?) -> LinkerSetting

Declares linkage to a system framework.

static func unsafeFlags([String], BuildSettingCondition?) -> LinkerSetting

Sets unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

