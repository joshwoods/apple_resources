

- Core Services
- File Metadata
-  MDSchema 

API Collection

# MDSchema

## Overview

The MDSchema functions provide information about the metadatareturned for an item including the type of metadata provided fora file type, the localized display name for a metadata attributekey, and the schema for a metadata attribute key.

## Topics

### MDSchema Miscellaneous Functions

func MDSchemaCopyAllAttributes() -> CFArray!

Returns an array containing all the metadata attributesdefined in the schema.

func MDSchemaCopyAttributesForContentType(CFString!) -> CFDictionary!

Returns a dictionary containing the metadata attributesfor the specified UTI type.

func MDSchemaCopyDisplayDescriptionForAttribute(CFString!) -> CFString!

Returns the localized description of a metadata attributekey.

func MDSchemaCopyDisplayNameForAttribute(CFString!) -> CFString!

Returns the localized display name of a metadata attributekey.

func MDSchemaCopyMetaAttributesForAttribute(CFString!) -> CFDictionary!

Returns a dictionary describing the values for the specifiedmetadata attribute key.

### Constants

Available Metadata Attribute Keys

Specify the available metadata attribute keys for a contenttype.

Metadata Attribute Schema Description Keys

Specify the schema of a metadata attribute key.

## See Also

### Opaque Types

MDItem

### Related Documentation

Spotlight Overview

