

- Core Services
- File Metadata
- MDSchema
-  MDSchemaCopyAttributesForContentType(\_:) 

Function

# MDSchemaCopyAttributesForContentType(\_:)

Returns a dictionary containing the metadata attributesfor the specified UTI type.

macOS 10.4+

``` source
func MDSchemaCopyAttributesForContentType(_ contentTypeUTI: CFString!) -> CFDictionary!
```

## Parameters 

`utiType`  

The UTI type.

## Return Value

A dictionary containing `kMDAttributeDisplayValues` and `kMDAttributeAllValues` keys.Returns `NULL` if the UTItype is unknown.

## Discussion

This function returns the metadata attributes for the specifiedUTI type only.

## See Also

### MDSchema Miscellaneous Functions

func MDSchemaCopyAllAttributes() -> CFArray!

Returns an array containing all the metadata attributesdefined in the schema.

func MDSchemaCopyDisplayDescriptionForAttribute(CFString!) -> CFString!

Returns the localized description of a metadata attributekey.

func MDSchemaCopyDisplayNameForAttribute(CFString!) -> CFString!

Returns the localized display name of a metadata attributekey.

func MDSchemaCopyMetaAttributesForAttribute(CFString!) -> CFDictionary!

Returns a dictionary describing the values for the specifiedmetadata attribute key.

