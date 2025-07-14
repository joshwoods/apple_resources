

- Core Foundation
-  CFXMLAttributeListDeclarationInfo 

Structure

# CFXMLAttributeListDeclarationInfo

Contains a list of the attributes associated with an element.

macOS

``` source
struct CFXMLAttributeListDeclarationInfo
```

## Overview

A pointer to this structure is included in the CFXMLNode object passed to your application when the parser encounters an attribute declaration in the DTD. Use the CFXMLNodeGetInfoPtr function to obtain the pointer to this structure.

## Topics

### Initializers

init()

init(numberOfAttributes: CFIndex, attributes: UnsafeMutablePointer&lt;CFXMLAttributeDeclarationInfo>!)

### Instance Properties

var attributes: UnsafeMutablePointer&lt;CFXMLAttributeDeclarationInfo>!

A C array of attributes.

var numberOfAttributes: CFIndex

The number of attributes in the array.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFXMLAttributeDeclarationInfo

Contains information about an element attribute definition.

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

