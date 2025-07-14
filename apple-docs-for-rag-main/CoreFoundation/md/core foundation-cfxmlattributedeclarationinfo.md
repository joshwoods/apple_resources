

- Core Foundation
-  CFXMLAttributeDeclarationInfo 

Structure

# CFXMLAttributeDeclarationInfo

Contains information about an element attribute definition.

macOS

``` source
struct CFXMLAttributeDeclarationInfo
```

## Overview

This structure is part of the definition of the CFXMLAttributeListDeclarationInfo structure.

## Topics

### Initializers

init()

init(attributeName: Unmanaged&lt;CFString>!, typeString: Unmanaged&lt;CFString>!, defaultString: Unmanaged&lt;CFString>!)

### Instance Properties

var attributeName: Unmanaged&lt;CFString>!

The name of the attribute.

var defaultString: Unmanaged&lt;CFString>!

The attribute’s default value.

var typeString: Unmanaged&lt;CFString>!

Describes the declaration of a single attribute.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

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

struct CFXMLExternalID

Contains the system and public IDs for an external entity reference.

struct CFXMLNotationInfo

Contains the external ID of the notation.

struct CFXMLProcessingInstructionInfo

Contains the text of the processing instruction.

