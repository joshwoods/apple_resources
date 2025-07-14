

- Foundation
-  XMLNode 

Class

# XMLNode

The nodes in the abstract, logical tree structure that represents an XML document.

Mac Catalyst 13.0+macOS 10.0+

``` source
class XMLNode
```

## Overview

Node objects can be of different kinds, corresponding to the following markup constructs in an XML document: element, attribute, text, processing instruction, namespace, and comment. In addition, a document-node object (specifically, an instance of XMLDocument) represents an XML document in its entirety. XMLNode objects can also represent document type declarations as well as declarations in Document Type Definitions (DTDs). Class factory methods of XMLNode enable you to create nodes of each kind. Only document, element, and DTD nodes may have child nodes.

Among the XML family of classes (excluding XMLParser) the XMLNode class is the base class. Inheriting from it are the classes XMLElement, XMLDocument, XMLDTD, and XMLDTDNode. XMLNode specifies the interface common to all XML node objects and defines common node behavior and attributes, for example hierarchy level, node name and value, tree traversal, and the ability to emit representative XML markup text.

### Subclassing Notes

You can subclass XMLNode if you want nodes of kinds different from the supported ones, You can also create a subclass with more specialized attributes or behavior than XMLNode.

#### Methods to Override

To subclass XMLNode you need to override the primary initializer, init(kind:options:), and the methods listed below. In most cases, you need only invoke the superclass implementation, adding any subclass-specific code before or after the invocation, as necessary.

| kind | parent |
|----|----|
| name | child(at:) |
| name | childCount |
| objectValue | children |
| objectValue | detach() |
| stringValue | localName |
| setStringValue(_:resolvingEntities:) | prefix |
| index | uri |

By default XMLNode implements the `NSObject` isEqual(_:) method to perform a deep comparison: two XMLNode objects are not considered equal unless they have the same name, same child nodes, same attributes, and so on. The comparison looks at the node and its children, but does not include the node’s parent. If you want a different standard of comparison, override `isEqual:`.

#### Special Considerations

Because of the architecture and data model of NSXML, when it parses and processes a source of XML it cannot know about your subclass unless you override the XMLDocument class method replacementClass(for:) to return your custom class in place of an NSXML class. If your custom class has no direct NSXML counterpart—for example, it is a subclass of XMLNode that represents CDATA sections—then you can walk the tree after it has been created and insert the new node where appropriate.

## Topics

### Creating and Initializing Node Objects

convenience init(kind: XMLNode.Kind)

Returns an `NSXMLNode` instance initialized with the constant indicating node kind.

init(kind: XMLNode.Kind, options: XMLNode.Options)

Returns an `NSXMLNode` instance initialized with the constant indicating node kind and one or more initialization options.

class func document() -> Any

Returns an empty document node.

class func document(withRootElement: XMLElement) -> Any

Returns an XMLDocument object initialized with a given root element.

class func element(withName: String) -> Any

Returns an XMLElement object with a given tag identifier, or name

class func element(withName: String, children: [XMLNode]?, attributes: [XMLNode]?) -> Any

Returns an XMLElement object with the given tag (name), attributes, and children.

class func element(withName: String, stringValue: String) -> Any

Returns an XMLElement object with a single text-node child containing the specified text.

class func element(withName: String, uri: String) -> Any

Returns an element whose fully qualified name is specified.

class func attribute(withName: String, stringValue: String) -> Any

Returns an `NSXMLNode` object representing an attribute node with a given name and string.

class func attribute(withName: String, uri: String, stringValue: String) -> Any

Returns an `NSXMLNode` object representing an attribute node with a given qualified name and string.

class func text(withStringValue: String) -> Any

Returns an `NSXMLNode` object representing a text node with specified content.

class func comment(withStringValue: String) -> Any

Returns an XMLNode object representing a comment node containing given text.

class func namespace(withName: String, stringValue: String) -> Any

Returns an `NSXMLNode` object representing a namespace with a specified name and URI.

class func dtdNode(withXMLString: String) -> Any?

Returns a XMLDTDNode object representing the DTD declaration for an element, attribute, entity, or notation based on a given string.

class func predefinedNamespace(forPrefix: String) -> XMLNode?

Returns an `NSXMLNode` object representing one of the predefined namespaces with the specified prefix.

class func processingInstruction(withName: String, stringValue: String) -> Any

Returns an `NSXMLNode` object representing a processing instruction with a specified name and value.

### Managing XML Node Objects

var index: Int

Returns the index of the receiver identifying its position relative to its sibling nodes.

var kind: XMLNode.Kind

Returns the kind of node the receiver is as a constant of type XMLNode.Kind.

var level: Int

Returns the nesting level of the receiver within the tree hierarchy.

var name: String?

Returns the name of the receiver.

var objectValue: Any?

Returns the object value of the receiver.

var stringValue: String?

Returns the content of the receiver as a string value.

func setStringValue(String, resolvingEntities: Bool)

Sets the content of the receiver as a string value and, optionally, resolves character references, predefined entities, and user-defined entities as declared in the associated DTD.

var uri: String?

Returns the URI associated with the receiver.

### Navigating the Tree of Nodes

var rootDocument: XMLDocument?

Returns the XMLDocument object containing the root element and representing the XML document as a whole.

var parent: XMLNode?

Returns the parent node of the receiver.

func child(at: Int) -> XMLNode?

Returns the child node of the receiver at the specified location.

var childCount: Int

Returns the number of child nodes the receiver has.

var children: [XMLNode]?

Returns an immutable array containing the child nodes of the receiver (as `NSXMLNode` objects).

var next: XMLNode?

Returns the next `NSXMLNode` object in document order.

var nextSibling: XMLNode?

Returns the next `NSXMLNode` object that is a sibling node to the receiver.

var previous: XMLNode?

Returns the previous `NSXMLNode` object in document order.

var previousSibling: XMLNode?

Returns the previous `NSXMLNode` object that is a sibling node to the receiver.

func detach()

Detaches the receiver from its parent node.

### Emitting Node Content

var xmlString: String

Returns the string representation of the receiver as it would appear in an XML document.

func xmlString(options: XMLNode.Options) -> String

Returns the string representation of the receiver as it would appear in an XML document, with one or more output options specified.

func canonicalXMLStringPreservingComments(Bool) -> String

Returns a string object encapsulating the receiver’s XML in canonical form.

var description: String

### Executing Queries

func nodes(forXPath: String) throws -> [XMLNode]

Returns the nodes resulting from executing an XPath query upon the receiver.

func objects(forXQuery: String) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

func objects(forXQuery: String, constants: [String : Any]?) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

var xPath: String?

Returns the XPath expression identifying the receiver’s location in the document tree.

### Managing Namespaces

var localName: String?

Returns the local name of the receiver.

class func localName(forName: String) -> String

Returns the local name from the specified qualified name.

var prefix: String?

Returns the prefix of the receiver’s name.

class func prefix(forName: String) -> String?

Returns the prefix from the specified qualified name.

### Constants

enum Kind

`NSXMLNode` declares the following constants of type NSXMLNodeKind for specifying a node’s kind in the initializer methods init(kind:) and init(kind:options:):

struct Options

These constants are input and output options for all `NSXMLNode` objects (unless otherwise indicated), including XMLDocument objects. You can specify these options in the `NSXMLNode` methods init(kind:options:) and xmlString(options:).

### Initializers

init()

## Relationships

### Inherits From

- NSObject

### Inherited By

- XMLDTD
- XMLDTDNode
- XMLDocument
- XMLElement

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

class XMLElement

The element nodes in an XML tree structure.

