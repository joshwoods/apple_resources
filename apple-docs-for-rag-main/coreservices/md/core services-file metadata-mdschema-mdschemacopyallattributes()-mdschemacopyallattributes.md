

- Core Services
- File Metadata
- MDSchema
-  MDSchemaCopyAllAttributes() 

Function

# MDSchemaCopyAllAttributes()

Returns an array containing all the metadata attributesdefined in the schema.

macOS 10.4+

``` source
func MDSchemaCopyAllAttributes() -> CFArray!
```

## See Also

### MDSchema Miscellaneous Functions

func MDSchemaCopyAttributesForContentType(CFString!) -> CFDictionary!

Returns a dictionary containing the metadata attributesfor the specified UTI type.

func MDSchemaCopyDisplayDescriptionForAttribute(CFString!) -> CFString!

Returns the localized description of a metadata attributekey.

func MDSchemaCopyDisplayNameForAttribute(CFString!) -> CFString!

Returns the localized display name of a metadata attributekey.

func MDSchemaCopyMetaAttributesForAttribute(CFString!) -> CFDictionary!

Returns a dictionary describing the values for the specifiedmetadata attribute key.

