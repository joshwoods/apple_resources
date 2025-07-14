

- Core Foundation
-  CFXMLNode 

Class

# CFXMLNode

macOS

``` source
class CFXMLNode
```

## Overview

A CFXMLNode object describes an individual XML construct—like a tag, or a comment, or a string of character data. CFXMLNode is intended to be used with the CFXMLParser and CFXMLTree opaque types.

Each CFXMLNode object contains three main pieces of information—the node’s type, the data string, and a pointer to an additional information data structure. A CFXMLNode object’s type is one of the enumerations described in CFXMLNodeTypeCode. The data string is always a CFString object; the meaning of the string is dependent on the node’s type. The format of the additional data is also dependent on the node’s type; in general, there is a custom structure for each type that requires additional data. See CFXMLNodeTypeCode for the mapping from a node type to meaning of the data string, and structure of the additional information. Note that these structures are versioned and may change as the parser changes. The current version can always be identified by the kCFXMLNodeCurrentVersion constant; earlier versions can be identified and used by passing earlier values for the version number (although the older structures would have been removed from the header).

You create a CFXMLNode object using one of the create or copy functions. Use the CFXMLNodeGetTypeCode, CFXMLNodeGetString, and CFXMLNodeGetInfoPtr functions to get the node type, data string, and additional information respectively. Use the CFXMLNodeGetVersion function to get a node’s version number.

## Topics

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

struct CFXMLExternalID

Contains the system and public IDs for an external entity reference.

struct CFXMLNotationInfo

Contains the external ID of the notation.

struct CFXMLProcessingInstructionInfo

Contains the text of the processing instruction.

### Constants

enum CFXMLEntityTypeCode

The entity type identification codes that the parser uses to describe XML entities.

Node Current Version

The version of a CFXMLNode object.

enum CFXMLNodeTypeCode

The various XML data type identification codes that the parser uses to describe XML structures.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

XML Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

