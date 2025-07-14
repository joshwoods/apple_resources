

- Core Foundation
-  CFXMLElementInfo 

Structure

# CFXMLElementInfo

Contains a list of element attributes packaged as CFDictionary key/value pairs.

macOS

``` source
struct CFXMLElementInfo
```

## Overview

A pointer to this structure is included in the CFXMLNode object passed to your application when the parser encounters an element containing attributes. Use the CFXMLNodeGetInfoPtr function to obtain the pointer.

## Topics

### Initializers

init()

### Instance Properties

var attributeOrder: Unmanaged&lt;CFArray>!

An array specifying the order in which the attributes appeared in the XML document.

var attributes: Unmanaged&lt;CFDictionary>!

The dictionary of attribute values.

var isEmpty: DarwinBoolean

A flag indicating whether the element was expressed in closed form.

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

