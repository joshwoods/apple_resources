

- Core Foundation
-  CFXMLEntityTypeCode 

Enumeration

# CFXMLEntityTypeCode

The entity type identification codes that the parser uses to describe XML entities.

macOS

``` source
enum CFXMLEntityTypeCode
```

## Overview

These codes are used with the CFXMLEntityInfo and CFXMLEntityReferenceInfo structures.

## Topics

### Constants

case parameter

Implies a parsed, internal entity.

case parsedInternal

Indicates a parsed, internal entity.

case parsedExternal

Indicates a parsed, external entity.

case unparsed

Indicates an unparsed entity.

case character

Indicates a character entity type.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Node Current Version

The version of a CFXMLNode object.

enum CFXMLNodeTypeCode

The various XML data type identification codes that the parser uses to describe XML structures.

