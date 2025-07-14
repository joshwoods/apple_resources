

- Core Services
- File Metadata
- MDSchema
-  MDSchemaCopyMetaAttributesForAttribute(\_:) 

Function

# MDSchemaCopyMetaAttributesForAttribute(\_:)

Returns a dictionary describing the values for the specifiedmetadata attribute key.

macOS 10.4+

``` source
func MDSchemaCopyMetaAttributesForAttribute(_ name: CFString!) -> CFDictionary!
```

## Parameters 

`name`  

The name of the metadata attribute key.

## Return Value

A dictionary describingthe schema of the metadata attribute key.

## See Also

### MDSchema Miscellaneous Functions

func MDSchemaCopyAllAttributes() -> CFArray!

Returns an array containing all the metadata attributesdefined in the schema.

func MDSchemaCopyAttributesForContentType(CFString!) -> CFDictionary!

Returns a dictionary containing the metadata attributesfor the specified UTI type.

func MDSchemaCopyDisplayDescriptionForAttribute(CFString!) -> CFString!

Returns the localized description of a metadata attributekey.

func MDSchemaCopyDisplayNameForAttribute(CFString!) -> CFString!

Returns the localized display name of a metadata attributekey.

