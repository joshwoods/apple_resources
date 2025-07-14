

- Foundation
-  XMLDTD 

Class

# XMLDTD

A representation of a Document Type Definition.

Mac Catalyst 13.0+macOS 10.0+

``` source
class XMLDTD
```

## Overview

An instance of the XMLDTD class is held as a property of an XMLDocument instance, accessed through the XMLDocument property dtd.

In the data model, an XMLDTD object is conceptually similar to namespace and attribute nodes: it is not considered to be a child of the XMLDocument object although it is closely associated with it. It is at the “root” of a shallow tree consisting primarily of nodes representing DTD declarations. Acceptable child nodes are instances of the XMLDTDNode class as well as XMLNode objects representing comment nodes and processing-instruction nodes.

You create an `NSXMLDTD` object in one of three ways:

- By processing an XML document with its own internal (in-line) DTD

- By process a standalone (external) DTD

- Programmatically

Once an XMLDTD instance is in place, you can add, remove, and change the XMLDTDNode objects representing various DTD declarations. When you write the document out as XML, the new or modified internal DTD is included (assuming you set the DTD in the XMLDocument instance). You may also programmatically create an external DTD and write that out to its own file.

## Topics

### Initializing an NSXMLDTD Object

convenience init(contentsOf: URL, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDTD` object created from the DTD declarations in a URL-referenced source.

init(data: Data, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDTD` object created from the DTD declarations encapsulated in an NSData object

### Managing DTD Identifiers

var publicID: String?

Returns the receiver’s public identifier.

var systemID: String?

Returns the receiver’s system identifier.

### Manipulating Child Nodes

func addChild(XMLNode)

Adds a child node to the end of the list of existing children.

func insertChild(XMLNode, at: Int)

Inserts a child node in the receiver’s list of children at a specific location in the list.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node at a particular location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child at a particular index with another child.

func setChildren([XMLNode]?)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

### Getting DTD Nodes by Name

class func predefinedEntityDeclaration(forName: String) -> XMLDTDNode?

Returns a DTD node representing the predefined entity declaration with the specified name.

func elementDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing an element declaration for a specified element.

func attributeDeclaration(forName: String, elementName: String) -> XMLDTDNode?

Returns the DTD node representing an attribute-list declaration for a given attribute and its element.

func entityDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the entity declaration for a specified entity.

func notationDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the notation declaration identified by the specified notation name.

### Initializers

init()

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

class XMLDTDNode

A representation of element, attribute-list, entity, and notation declarations in a Document Type Definition.

class XMLDocument

An XML document as internalized into a logical tree structure.

class XMLElement

The element nodes in an XML tree structure.

class XMLNode

The nodes in the abstract, logical tree structure that represents an XML document.

