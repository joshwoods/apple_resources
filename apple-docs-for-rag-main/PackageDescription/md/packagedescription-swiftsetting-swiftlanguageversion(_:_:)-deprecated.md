

- PackageDescription
- SwiftSetting
-  swiftLanguageVersion(\_:\_:) Deprecated

Type Method

# swiftLanguageVersion(\_:\_:)

Defines a `-swift-version` to pass to the corresponding build tool.

SwiftPM 6.0–6.0Deprecated

``` source
static func swiftLanguageVersion(
    _ version: SwiftVersion,
    _ condition: BuildSettingCondition? = nil
) -> SwiftSetting
```

## Parameters 

`version`  

The Swift language version to use.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

Since

First available in PackageDescription 6.0.

