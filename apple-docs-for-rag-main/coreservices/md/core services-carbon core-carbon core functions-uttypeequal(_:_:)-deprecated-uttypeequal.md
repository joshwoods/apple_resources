

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeEqual(\_:\_:) Deprecated

Function

# UTTypeEqual(\_:\_:)

Returns whether two uniform type identifiers are equal.

iOS 3.0–15.0DeprecatediPadOS 3.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.3–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
func UTTypeEqual(
    _ inUTI1: CFString,
    _ inUTI2: CFString
) -> Bool
```

## Parameters 

`inUTI1`  

A uniform type identifier.

`inUTI2`  

The uniform type identifier to compare it to.

## Return Value

Returns `true` if the two uniform type identifiers are equivalent.

