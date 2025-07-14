

- PackageDescription
- SwiftSetting
-  enableUpcomingFeature(\_:\_:) 

Type Method

# enableUpcomingFeature(\_:\_:)

Enable an upcoming feature with the given name.

SwiftPM 5.8+

``` source
static func enableUpcomingFeature(
    _ name: String,
    _ condition: BuildSettingCondition? = nil
) -> SwiftSetting
```

## Parameters 

`name`  

The name of the upcoming feature; for example, `ConciseMagicFile`.

`condition`  

A condition that restricts the application of the build setting.

## Discussion

An upcoming feature is one that is available in Swift as of a certain language version, but isn’t available by default in prior language modes because it has some impact on source compatibility.

You can add and use multiple upcoming features in a given target without affecting its dependencies. Targets will ignore any unknown upcoming features.

Since

First available in PackageDescription 5.8.

