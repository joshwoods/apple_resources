

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeConformsTo(\_:\_:) Deprecated

Function

# UTTypeConformsTo(\_:\_:)

Returns whether a uniform type identifier conforms to another uniform type identifier.

iOS 3.0–15.0DeprecatediPadOS 3.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.3–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
func UTTypeConformsTo(
    _ inUTI: CFString,
    _ inConformsToUTI: CFString
) -> Bool
```

## Parameters 

`inUTI`  

A uniform type identifier to compare.

`inConformsToUTI`  

The uniform type identifier to compare it to.

## Return Value

Returns `true` if the uniform type identifier is equal to or conforms to the second type.

