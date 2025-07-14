

- PackageDescription
- SwiftSetting
-  define(\_:\_:) 

Type Method

# define(\_:\_:)

Defines a compilation condition.

SwiftPM 5.0+

``` source
static func define(
    _ name: String,
    _ condition: BuildSettingCondition? = nil
) -> SwiftSetting
```

## Parameters 

`name`  

The name of the macro.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

Use compilation conditions to only compile statements if a certain condition is true. For example, the Swift compiler will only compile the statements inside the `#if` block when `ENABLE_SOMETHING` is defined:

```
#if ENABLE_SOMETHING
   ...
#endif
```

Unlike macros in C/C++, compilation conditions don’t have an associated value.

Since

First available in PackageDescription 5.0.

## See Also

### Configuring Swift Settings

static func unsafeFlags([String], BuildSettingCondition?) -> SwiftSetting

Set unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

