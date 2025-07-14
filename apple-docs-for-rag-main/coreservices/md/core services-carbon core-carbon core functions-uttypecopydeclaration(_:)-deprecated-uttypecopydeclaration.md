

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeCopyDeclaration(\_:) Deprecated

Function

# UTTypeCopyDeclaration(\_:)

Returns a uniform type’s declaration.

iOS 3.0–15.0DeprecatediPadOS 3.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.3–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
func UTTypeCopyDeclaration(_ inUTI: CFString) -> Unmanaged?
```

## Parameters 

`inUTI`  

A uniform type identifier.

## Return Value

A dictionary that contains the uniform type’s declaration, or `NULL` if no declaration for that type can be found.

## Discussion

A uniform type identifier is declared in a bundle’s information Property list (`info.plist`). This function extracts and returns a dictionary that contains the complete declaration of the uniform type identifier. This is useful when your application needs to access properties that does not have a built-in accessor function. For more information on the dictionary format, see Uniform Type Identifiers Overview.

