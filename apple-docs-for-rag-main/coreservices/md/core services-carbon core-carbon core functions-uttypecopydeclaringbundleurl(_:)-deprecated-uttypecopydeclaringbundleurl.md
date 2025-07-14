

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeCopyDeclaringBundleURL(\_:) Deprecated

Function

# UTTypeCopyDeclaringBundleURL(\_:)

Returns the location of a bundle containing the declaration for a type.

iOS 3.0–14.0DeprecatediPadOS 3.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.3–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–7.0Deprecated

``` source
func UTTypeCopyDeclaringBundleURL(_ inUTI: CFString) -> Unmanaged?
```

## Parameters 

`inUTI`  

A uniform type identifier.

## Return Value

A URL that points to the bundle that holds the uniform type identifier’s declaration, or `NULL` if a bundle that holds the declaration cannot be located.

