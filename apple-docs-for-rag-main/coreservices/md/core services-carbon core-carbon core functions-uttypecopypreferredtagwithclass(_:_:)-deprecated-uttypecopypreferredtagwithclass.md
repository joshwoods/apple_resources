

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeCopyPreferredTagWithClass(\_:\_:) Deprecated

Function

# UTTypeCopyPreferredTagWithClass(\_:\_:)

Translates a uniform type identifier to a list of tags in a different type classification method.

iOS 3.0–15.0DeprecatediPadOS 3.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.3–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
func UTTypeCopyPreferredTagWithClass(
    _ inUTI: CFString,
    _ inTagClass: CFString
) -> Unmanaged?
```

## Parameters 

`inUTI`  

The uniform type identifier to convert.

`inTagClass`  

The class of the tags you want to return. For more information, see `Type Tag Classes`.

## Return Value

An array of tags (as CFStrings), or `NULL` if there was no translation available to convert the uniform type identifier to the specified class.

## Discussion

If the type declaration included more than one tag with the specified class, the first tag in the declared tag array is the preferred tag.

