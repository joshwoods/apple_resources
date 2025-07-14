

- Core Foundation
-  CFXMLExternalID 

Structure

# CFXMLExternalID

Contains the system and public IDs for an external entity reference.

macOS

``` source
struct CFXMLExternalID
```

## Overview

This structure is part of the definition of the CFXMLDocumentTypeInfo, CFXMLNotationInfo, and CFXMLEntityInfo structures.

## Topics

### Initializers

init()

init(systemID: Unmanaged&lt;CFURL>!, publicID: Unmanaged&lt;CFString>!)

### Instance Properties

var publicID: Unmanaged&lt;CFString>!

The publicID string.

var systemID: Unmanaged&lt;CFURL>!

The systemID URL.

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

struct CFXMLEntityInfo

Contains information describing an XML entity.

struct CFXMLEntityReferenceInfo

Contains information describing an XML entity reference.

struct CFXMLNotationInfo

Contains the external ID of the notation.

struct CFXMLProcessingInstructionInfo

Contains the text of the processing instruction.

