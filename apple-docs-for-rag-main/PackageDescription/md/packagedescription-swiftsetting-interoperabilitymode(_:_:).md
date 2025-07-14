

- PackageDescription
- SwiftSetting
-  interoperabilityMode(\_:\_:) 

Type Method

# interoperabilityMode(\_:\_:)

Enable Swift interoperability with a given language.

SwiftPM 5.9+

``` source
static func interoperabilityMode(
    _ mode: SwiftSetting.InteroperabilityMode,
    _ condition: BuildSettingCondition? = nil
) -> SwiftSetting
```

## Parameters 

`mode`  

The language mode, either C or Cxx.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

This is useful for enabling interoperability between Swift and C++ for a given target.

Enabling C++ interoperability mode might alter the way some existing C and Objective-C APIs are imported.

Since

First available in PackageDescription 5.9.

