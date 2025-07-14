

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTTypeCreatePreferredIdentifierForTag(\_:\_:\_:) Deprecated

Function

# UTTypeCreatePreferredIdentifierForTag(\_:\_:\_:)

Creates a uniform type identifier for the type indicated by the specified tag.

iOS 3.0–15.0DeprecatediPadOS 3.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.3–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
func UTTypeCreatePreferredIdentifierForTag(
    _ inTagClass: CFString,
    _ inTag: CFString,
    _ inConformingToUTI: CFString?
) -> Unmanaged?
```

## Parameters 

`inTagClass`  

The class of the `inTag` parameter. For more information, see `Type Tag Classes`.

`inTag`  

The tag to translate into a uniform type identifier.

`inConformingToUTI`  

If not `NULL`, the returned uniform type identifier must conform to this parameter.

## Return Value

A new CFStringRef containing a uniform type identifier, or `NULL` if inTagClass is not a known tag class

## Discussion

This function is used to translate a type declared using another declaration mechanism (for example, MIME types) into a uniform type identifier. This function searches all UTI declarations for a matching translation. If a conforming parameter is assigned, the search is reduced to the subset of type identifiers that conform to that type.

If there is more than one possible UTI for the specified tag, the UTI that will be returned is undefined. See UTTypeCreateAllIdentifiersForTag(_:_:_:) if you need to see all search results.

If no result is found, this function creates a dynamic type beginning with the `dyn` prefix. This allows you to pass the UTI around and convert it back to the original tag.

## See Also

### Related Documentation

func UTTypeCopyPreferredTagWithClass(CFString, CFString) -> Unmanaged&lt;CFString>?

Translates a uniform type identifier to a list of tags in a different type classification method.

Uniform Type Identifiers Overview

