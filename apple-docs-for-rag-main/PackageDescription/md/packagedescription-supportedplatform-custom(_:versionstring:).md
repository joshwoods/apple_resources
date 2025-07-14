

- PackageDescription
- SupportedPlatform
-  custom(\_:versionString:) 

Type Method

# custom(\_:versionString:)

Configures the minimum deployment target version for custom platforms.

SwiftPM 5.6+

``` source
static func custom(
    _ platformName: String,
    versionString: String
) -> SupportedPlatform
```

## Parameters 

`platformName`  

The name of the platform.

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `19.0.1`.

## Return Value

A `SupportedPlatform` instance.

## Discussion

Since

First available in PackageDescription 5.6

