

- Foundation
-  XMLElement 

Class

# XMLElement

The element nodes in an XML tree structure.

Mac Catalyst 13.0+macOS 10.0+

``` source
class XMLElement
```

## Mentioned in 

setURI:

## Overview

An XMLElement object may have child nodes, specifically comment nodes, processing-instruction nodes, text nodes, and other XMLElement nodes. It may also have attribute nodes and namespace nodes associated with it (however, namespace and attribute nodes are not considered children). Any attempt to add a XMLDocument node, XMLDTD node, namespace node, or attribute node as a child raises an exception. If you add a child node to an XMLElement object and that child already has a parent, XMLElement raises an exception; the child must be detached or copied first.

### Subclassing Notes

You can subclass `NSXMLElement` if you want element nodes with more specialized attributes or behavior, for example, paragraph and font attributes that specify how the string value of the element should appear.

#### Methods to Override

To subclass `NSXMLElement` you need to override the primary initializer, init(name:uri:), and the methods listed below. In most cases, you need only invoke the superclass implementation, adding any subclass-specific code before or after the invocation, as necessary.

| addAttribute(_:) | removeNamespace(forPrefix:) |
|----|----|
| removeAttribute(forName:) | namespaces |
| attributes | namespaces |
| attribute(forLocalName:uri:) | insertChild(_:at:) |
| attributes | removeChild(at:) |
| addNamespace(_:) | setChildren(_:) |

`NSXMLElement` implements isEqual(_:) to perform a deep comparison: two XMLDocument objects are not considered equal unless they have the same name, same child nodes, same attributes, and so on. If you want a different standard of comparison, override `isEqual:`.

#### Special Considerations

Because of the architecture and data model of NSXML, when it parses and processes a source of XML it cannot know about your subclass unless you override the class method replacementClass(for:) to return your custom class in place of an NSXML class. If your custom class has no direct NSXML counterpart—for example, it is a subclass of `NSXMLNode` that represents CDATA sections—then you can walk the tree after it has been created and insert the new node where appropriate.

Note that you can safely set the root element of the XML document (using the `NSXMLDocument` setRootElement(_:)method) to be an instance of your subclass because this method only checks to see if the added node is of an element kind (`NSXMLElementKind`). These precautions do not apply, of course, if you are creating an XML tree programmatically.

## Topics

### Initializing NSXMLElement Objects

convenience init(name: String)

Returns an `NSXMLElement` object initialized with the specified name.

convenience init(name: String, stringValue: String?)

Returns an `NSXMLElement` object initialized with a specified name and a single text-node child containing a specified value.

init(name: String, uri: String?)

Returns an `NSXMLElement` object initialized with the specified name and URI.

init(xmlString: String) throws

Returns an `NSXMLElement` object created from a specified string containing XML markup.

convenience init(kind: XMLNode.Kind, options: XMLNode.Options)

### Obtaining Child Elements

func elements(forName: String) -> [XMLElement]

Returns the child element nodes (as `NSXMLElement` objects) of the receiver that have a specified name.

func elements(forLocalName: String, uri: String?) -> [XMLElement]

Returns the child element nodes (as `NSXMLElement` objects) of the receiver that are matched with the specified local name and URI.

### Manipulating Child Elements

func addChild(XMLNode)

Adds a child node at the end of the receiver’s current list of children.

func insertChild(XMLNode, at: Int)

Inserts a new child node at a specified location in the receiver’s list of child nodes.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node of the receiver identified by a given index.

func replaceChild(at: Int, with: XMLNode)

Replaces a child node at a specified location with another child node.

func setChildren([XMLNode]?)

Sets all child nodes of the receiver at once, replacing any existing children.

func normalizeAdjacentTextNodesPreservingCDATA(Bool)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

### Handling Attributes

func addAttribute(XMLNode)

Adds an attribute node to the receiver.

func attribute(forName: String) -> XMLNode?

Returns the attribute node of the receiver with the specified name.

func attribute(forLocalName: String, uri: String?) -> XMLNode?

Returns the attribute node of the receiver that is identified by a local name and URI.

var attributes: [XMLNode]?

Sets all attributes of the receiver at once, replacing any existing attribute nodes.

func removeAttribute(forName: String)

Removes an attribute node identified by name.

func setAttributesWith([String : String])

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

### Handling Namespaces

func addNamespace(XMLNode)

Adds a namespace node to the receiver.

var namespaces: [XMLNode]?

Sets all of the namespace nodes of the receiver at once, replacing any existing namespace nodes.

func namespace(forPrefix: String) -> XMLNode?

Returns the namespace node with a specified prefix.

func removeNamespace(forPrefix: String)

Removes a namespace node that is identified by a given prefix.

func resolveNamespace(forName: String) -> XMLNode?

Returns the namespace node with the prefix matching the given qualified name.

func resolvePrefix(forNamespaceURI: String) -> String?

Returns the prefix associated with the specified URI.

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

class XMLDTDNode

A representation of element, attribute-list, entity, and notation declarations in a Document Type Definition.

class XMLDocument

An XML document as internalized into a logical tree structure.

class XMLNode

The nodes in the abstract, logical tree structure that represents an XML document.

