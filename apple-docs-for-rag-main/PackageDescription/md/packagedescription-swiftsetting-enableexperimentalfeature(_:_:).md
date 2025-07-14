

- PackageDescription
- SwiftSetting
-  enableExperimentalFeature(\_:\_:) 

Type Method

# enableExperimentalFeature(\_:\_:)

Enable an experimental feature with the given name.

SwiftPM 5.8+

``` source
static func enableExperimentalFeature(
    _ name: String,
    _ condition: BuildSettingCondition? = nil
) -> SwiftSetting
```

## Parameters 

`name`  

The name of the experimental feature; for example, `VariadicGenerics`.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

An experimental feature is one that’s in development, but is not yet available in Swift as a language feature.

You can add and use multiple experimental features in a given target without affecting its dependencies. Targets will ignore any unknown experimental features.

Since

First available in PackageDescription 5.8.

