

- Foundation
- XMLNode
-  XMLNode.Kind 

Enumeration

# XMLNode.Kind

`NSXMLNode` declares the following constants of type NSXMLNodeKind for specifying a node’s kind in the initializer methods init(kind:) and init(kind:options:):

Mac Catalyst 13.0+macOS 10.0+

``` source
enum Kind
```

## Topics

### Constants

case invalid

Indicates a node object created without a valid kind being specified (as returned by the kind method).

case document

Specifies a document node.

case element

Specifies an element node.

case attribute

Specifies an attribute node

case namespace

Specifies a namespace node.

case processingInstruction

Specifies a processing-instruction node.

case comment

Specifies a comment node.

case text

Specifies a text node.

case DTDKind

Specifies a document-type declaration (DTD) node.

case entityDeclaration

Specifies an entity-declaration node.

case attributeDeclaration

Specifies an attribute-list declaration node.

case elementDeclaration

Specifies an element declaration node.

case notationDeclaration

Specifies a notation declaration node.

case invalid

Indicates a node object created without a valid kind being specified (as returned by the kind method).

case document

Specifies a document node.

case element

Specifies an element node.

case attribute

Specifies an attribute node

case namespace

Specifies a namespace node.

case processingInstruction

Specifies a processing-instruction node.

case comment

Specifies a comment node.

case text

Specifies a text node.

case DTDKind

Specifies a document-type declaration (DTD) node.

case entityDeclaration

Specifies an entity-declaration node.

case attributeDeclaration

Specifies an attribute-list declaration node.

case elementDeclaration

Specifies an element declaration node.

case notationDeclaration

Specifies a notation declaration node.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct Options

These constants are input and output options for all `NSXMLNode` objects (unless otherwise indicated), including XMLDocument objects. You can specify these options in the `NSXMLNode` methods init(kind:options:) and xmlString(options:).

