

- Core Services
- File Metadata
- MDSchema
-  MDSchemaCopyDisplayNameForAttribute(\_:) 

Function

# MDSchemaCopyDisplayNameForAttribute(\_:)

Returns the localized display name of a metadata attributekey.

macOS 10.4+

``` source
func MDSchemaCopyDisplayNameForAttribute(_ name: CFString!) -> CFString!
```

## Parameters 

`name`  

The name of the metadata attribute key.

## Return Value

The localized displayname of the metadata attribute, or `NULL` ifno localized display name is available.

## See Also

### MDSchema Miscellaneous Functions

func MDSchemaCopyAllAttributes() -> CFArray!

Returns an array containing all the metadata attributesdefined in the schema.

func MDSchemaCopyAttributesForContentType(CFString!) -> CFDictionary!

Returns a dictionary containing the metadata attributesfor the specified UTI type.

func MDSchemaCopyDisplayDescriptionForAttribute(CFString!) -> CFString!

Returns the localized description of a metadata attributekey.

func MDSchemaCopyMetaAttributesForAttribute(CFString!) -> CFDictionary!

Returns a dictionary describing the values for the specifiedmetadata attribute key.

