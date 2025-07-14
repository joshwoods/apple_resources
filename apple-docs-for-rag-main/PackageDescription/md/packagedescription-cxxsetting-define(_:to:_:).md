

- PackageDescription
- CXXSetting
-  define(\_:to:\_:) 

Type Method

# define(\_:to:\_:)

Defines a value for a macro.

SwiftPM 5.0+

``` source
static func define(
    _ name: String,
    to value: String? = nil,
    _ condition: BuildSettingCondition? = nil
) -> CXXSetting
```

## Parameters 

`name`  

The name of the macro.

`value`  

The value of the macro.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

If you don’t specify a value, the macro’s default value is 1.

Since

First available in PackageDescription 5.0.

## See Also

### Configuring CXX Settings

static func headerSearchPath(String, BuildSettingCondition?) -> CXXSetting

Provides a header search path relative to the target’s directory.

static func unsafeFlags([String], BuildSettingCondition?) -> CXXSetting

Sets unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

