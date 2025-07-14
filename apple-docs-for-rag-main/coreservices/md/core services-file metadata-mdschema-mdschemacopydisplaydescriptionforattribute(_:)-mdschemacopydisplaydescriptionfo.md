

- Core Services
- File Metadata
- MDSchema
-  MDSchemaCopyDisplayDescriptionForAttribute(\_:) 

Function

# MDSchemaCopyDisplayDescriptionForAttribute(\_:)

Returns the localized description of a metadata attributekey.

macOS 10.4+

``` source
func MDSchemaCopyDisplayDescriptionForAttribute(_ name: CFString!) -> CFString!
```

## Parameters 

`name`  

The name of the metadata attribute key.

## Return Value

The localized descriptionof the metadata attribute, or `NULL` ifno localized description is available.

## See Also

### MDSchema Miscellaneous Functions

func MDSchemaCopyAllAttributes() -> CFArray!

Returns an array containing all the metadata attributesdefined in the schema.

func MDSchemaCopyAttributesForContentType(CFString!) -> CFDictionary!

Returns a dictionary containing the metadata attributesfor the specified UTI type.

func MDSchemaCopyDisplayNameForAttribute(CFString!) -> CFString!

Returns the localized display name of a metadata attributekey.

func MDSchemaCopyMetaAttributesForAttribute(CFString!) -> CFDictionary!

Returns a dictionary describing the values for the specifiedmetadata attribute key.

