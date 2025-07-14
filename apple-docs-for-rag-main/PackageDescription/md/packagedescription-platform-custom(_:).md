

- PackageDescription
- Platform
-  custom(\_:) 

Type Method

# custom(\_:)

Creates a custom platform.

SwiftPM 5.6+

``` source
static func custom(_ platformName: String) -> Platform
```

## Parameters 

`platformName`  

The name of the platform.

## Return Value

A `Platform` instance.

## Discussion

Use this function if none of the predefined platform names match the platform you are targeting.

