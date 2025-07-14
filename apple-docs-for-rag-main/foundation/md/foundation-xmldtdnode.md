

- Foundation
-  XMLDTDNode 

Class

# XMLDTDNode

A representation of element, attribute-list, entity, and notation declarations in a Document Type Definition.

Mac Catalyst 13.0+macOS 10.0+

``` source
class XMLDTDNode
```

## Overview

XMLDTDNode objects are the sole children of a XMLDTD object (possibly along with comment nodes and processing-instruction nodes). They themselves cannot have any children.

XMLDTDNode objects can be of four kinds—element, attribute-list, entity, or notation declaration—and can also be of a subkind, as specified by a XMLDTDNode.DTDKind constant. For example, a DTD entity-declaration node could represent an unparsed entity declaration (XMLDTDNode.DTDKind.unparsed) rather than a parameter entity declaration (XMLDTDNode.DTDKind.parameter). You can use a DTD node’s subkind to help determine how to handle the value of the node.

You can create an XMLDTDNode object with the init(xmlString:) method, the XMLNode class method dtdNode(withXMLString:), or with the XMLNode initializer init(kind:options:) (in the latter method supplying the appropriate XMLNode.Kind constant).

Setting the object value or string value of an XMLDTDNode objects affects different parts of different kinds of declaration. See the related programming topic for more information.

## Topics

### Initializing an NSXMLDTDNode Object

init?(xmlString: String)

Returns an `NSXMLDTDNode` object initialized with the DTD declaration in a given string.

### Managing the DTD Node Kind

var dtdKind: XMLDTDNode.DTDKind

Returns the receiver’s DTD kind.

### Managing DTD Identifiers

var isExternal: Bool

var notationName: String?

Returns the name of the notation associated with the receiver.

var publicID: String?

Returns the public identifier associated with the receiver.

var systemID: String?

Returns the system identifier associated with the receiver.

### Constants

enum DTDKind

The type defined for the constants that specify the kind and subkind of DTD declaration represented by an `NSXMLDTDNode` object. You set the DTD-node kind using the doc:nsxmldtdnode/1806486-setdtdkind method.

DTD Node Kind Constants

Constants that specify the kind and subkind of DTD declaration represented by an `NSXMLDTDNode` object. You set the DTD-node kind using the doc:nsxmldtdnode/1806486-setdtdkind method.

### Initializers

init()

init(kind: XMLNode.Kind, options: XMLNode.Options)

## Relationships

### Inherits From

- XMLNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Tree-Based Processing

class XMLDTD

A representation of a Document Type Definition.

class XMLDocument

An XML document as internalized into a logical tree structure.

class XMLElement

The element nodes in an XML tree structure.

class XMLNode

The nodes in the abstract, logical tree structure that represents an XML document.

