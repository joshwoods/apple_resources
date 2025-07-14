

- Core Foundation
-  CFXMLDocumentTypeInfo 

Structure

# CFXMLDocumentTypeInfo

Contains the external ID of the DTD.

macOS

``` source
struct CFXMLDocumentTypeInfo
```

## Overview

A pointer to this structure is included in the CFXMLNode object passed to your application when the parser encounters the beginning of the DTD. Use the CFXMLNodeGetInfoPtr function to obtain a pointer to this structure.

## Topics

### Initializers

init()

init(externalID: CFXMLExternalID)

### Instance Properties

var externalID: CFXMLExternalID

The external ID of the DTD.

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

struct CFXMLElementInfo

Contains a list of element attributes packaged as CFDictionary key/value pairs.

struct CFXMLElementTypeDeclarationInfo

Contains a description of the element type.

struct CFXMLEntityInfo

Contains information describing an XML entity.

struct CFXMLEntityReferenceInfo

Contains information describing an XML entity reference.

struct CFXMLExternalID

Contains the system and public IDs for an external entity reference.

struct CFXMLNotationInfo

Contains the external ID of the notation.

struct CFXMLProcessingInstructionInfo

Contains the text of the processing instruction.

