

- Core Foundation
-  CFXMLEntityReferenceInfo 

Structure

# CFXMLEntityReferenceInfo

Contains information describing an XML entity reference.

macOS

``` source
struct CFXMLEntityReferenceInfo
```

## Overview

A pointer to this structure is included in the CFXMLNode object passed to your application when the parser encounters an entity reference. Use the CFXMLNodeGetInfoPtr function to obtain the pointer.

## Topics

### Initializers

init()

init(entityType: CFXMLEntityTypeCode)

### Instance Properties

var entityType: CFXMLEntityTypeCode

The entity type code.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

struct CFXMLEntityInfo

Contains information describing an XML entity.

struct CFXMLExternalID

Contains the system and public IDs for an external entity reference.

struct CFXMLNotationInfo

Contains the external ID of the notation.

struct CFXMLProcessingInstructionInfo

Contains the text of the processing instruction.

