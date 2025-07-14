

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeCopyDescription(\_:) Deprecated

Function

# UTTypeCopyDescription(\_:)

Returns the localized, user-readable type description string associated with a uniform type identifier.

iOS 3.0–15.0DeprecatediPadOS 3.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.3–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
func UTTypeCopyDescription(_ inUTI: CFString) -> Unmanaged?
```

## Parameters 

`inUTI`  

A uniform type identifier.

## Return Value

A localized string describing the type, or `NULL` if no type description is available.

## Discussion

The localized string that describes the uniform type is found in the type’s declaration.

