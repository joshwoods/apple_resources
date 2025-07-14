

- PackageDescription
- CSetting
-  unsafeFlags(\_:\_:) 

Type Method

# unsafeFlags(\_:\_:)

Sets unsafe flags to pass arbitrary command-line flags to the corresponding build tool.

SwiftPM 5.0+

``` source
static func unsafeFlags(
    _ flags: [String],
    _ condition: BuildSettingCondition? = nil
) -> CSetting
```

## Parameters 

`flags`  

The unsafe flags to set.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

As the usage of the word “unsafe” implies, Swift Package Manager can’t safely determine if the build flags have any negative side effect on the build since certain flags can change the behavior of how it performs a build.

As some build flags can be exploited for unsupported or malicious behavior, the use of unsafe flags makes the products containing this target ineligible for use by other packages.

Since

First available in PackageDescription 5.0.

## See Also

### Configuring C Settings

static func define(String, to: String?, BuildSettingCondition?) -> CSetting

Defines a value for a macro.

static func headerSearchPath(String, BuildSettingCondition?) -> CSetting

Provides a header search path relative to the target’s directory.

