

- Core Foundation
-  CFXMLEntityInfo 

Structure

# CFXMLEntityInfo

Contains information describing an XML entity.

macOS

``` source
struct CFXMLEntityInfo
```

## Overview

A pointer to this structure is included in the CFXMLNode object passed to your application when the parser encounters an entity declaration. Use the CFXMLNodeGetInfoPtr function to obtain a pointer to this structure.

## Topics

### Initializers

init()

init(entityType: CFXMLEntityTypeCode, replacementText: Unmanaged&lt;CFString>!, entityID: CFXMLExternalID, notationName: Unmanaged&lt;CFString>!)

### Instance Properties

var entityID: CFXMLExternalID

`entityID.systemID` will be `NULL` if `entityType` is internal.

var entityType: CFXMLEntityTypeCode

The entity type code.

var notationName: Unmanaged&lt;CFString>!

`NULL` if `entityType` is parsed.

var replacementText: Unmanaged&lt;CFString>!

`NULL` if `entityType` is external or unparsed, otherwise the text that the entity should be replaced with.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFXMLAttributeDeclarationInfo

Contains information about an element attribute definition.

struct CFXMLAttributeListDeclarationInfo

Contains a list of the attributes associated with an element.

struct CFXMLDocumentInfo

Contains the source URL and text encoding information for the XML document.

struct CFXMLDocumentTypeInfo

Contains the external ID of the DTD.

struct CFXMLElementInfo

Contains a list of element attributes packaged as CFDictionary key/value pairs.

struct CFXMLElementTypeDeclarationInfo

Contains a description of the element type.

struct CFXMLEntityReferenceInfo

Contains information describing an XML entity reference.

struct CFXMLExternalID

Contains the system and public IDs for an external entity reference.

struct CFXMLNotationInfo

Contains the external ID of the notation.

struct CFXMLProcessingInstructionInfo

Contains the text of the processing instruction.

