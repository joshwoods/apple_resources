

- PackageDescription
- SwiftSetting
-  swiftLanguageMode(\_:\_:) 

Type Method

# swiftLanguageMode(\_:\_:)

Defines a `-language-mode` to pass to the corresponding build tool.

SwiftPM 6.0+

``` source
static func swiftLanguageMode(
    _ mode: SwiftLanguageMode,
    _ condition: BuildSettingCondition? = nil
) -> SwiftSetting
```

## Parameters 

`mode`  

The Swift language mode to use.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

Since

First available in PackageDescription 6.0.

