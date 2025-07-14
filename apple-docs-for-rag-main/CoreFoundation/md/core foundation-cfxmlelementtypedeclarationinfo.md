

- Core Foundation
-  CFXMLElementTypeDeclarationInfo 

Structure

# CFXMLElementTypeDeclarationInfo

Contains a description of the element type.

macOS

``` source
struct CFXMLElementTypeDeclarationInfo
```

## Overview

A pointer to this structure is included in the CFXMLNode passed to your application when the parser encounters and element type declaration. Use the CFXMLNodeGetInfoPtr function to obtain a pointer to this structure.

## Topics

### Initializers

init()

init(contentDescription: Unmanaged&lt;CFString>!)

### Instance Properties

var contentDescription: Unmanaged&lt;CFString>!

A textual description of the element type.

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

