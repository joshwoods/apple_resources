

- Core Services
- File Metadata
- MDSchema
-  Metadata Attribute Schema Description Keys 

API Collection

# Metadata Attribute Schema Description Keys

Specify the schema of a metadata attribute key.

## Overview

These keys are in the dictionary returned by the function `MDSchemaCopyMetaAttributesForAttribute`.

## Topics

### Constants

let kMDAttributeName: CFString!

A string containing the name of the metadataattribute key.

let kMDAttributeType: CFString!

A CFNumberRef or CFTypeId describing thetype of data returned as the value of the metadata attribute key.

let kMDAttributeMultiValued: CFString!

A boolean that indicates if the metadataattribute value is multi-valued. If this is `TRUE`,the metadata attribute value is an array of the types specifiedin `kMDAttributeType`.

