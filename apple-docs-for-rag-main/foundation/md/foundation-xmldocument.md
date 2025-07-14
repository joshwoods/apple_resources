

- Foundation
-  XMLDocument 

Class

# XMLDocument

An XML document as internalized into a logical tree structure.

Mac Catalyst 13.0+macOS 10.0+

``` source
class XMLDocument
```

## Mentioned in 

setURI:

## Overview

An XMLDocument object can have multiple child nodes but only one element, the root element. Any other node must be a XMLNode object representing a comment or a processing instruction. If you attempt to add any other kind of child node to an XMLDocument object, such as an attribute, namespace, another document object, or an element other than the root, XMLDocument raises an exception. If you add a valid child node and that object already has a parent, XMLDocument raises an exception. An XMLDocument object may also have document-global attributes, such as XML version, character encoding, referenced DTD, and MIME type.

The initializers of the XMLDocument class read an external source of XML, whether it be a local file or remote website, parse it, and process it into the tree representation. You can also construct an XMLDocument programmatically. There are accessor methods for getting and setting document attributes, methods for transforming documents using XSLT, a method for dynamically validating a document, and methods for printing out the content of an XMLDocument as XML, XHTML, HTML, or plain text.

The XMLDocument class is thread-safe as long as any given instance is used only in one thread.

### Subclassing Notes

#### Methods to Override

To subclass `NSXMLDocument` you need to override the primary initializer, init(data:options:), and the methods listed below. In most cases, you need only invoke the superclass implementation, adding any subclass-specific code before or after the invocation, as necessary.

- rootElement()

- setChildren(_:)

- removeChild(at:)

- insertChild(_:at:)

- characterEncoding

- characterEncoding

- documentContentKind

- documentContentKind

- dtd

- mimeType

- isStandalone

- version

- version

By default `NSXMLDocument` implements the `NSObject` isEqual(_:) method to perform a deep comparison: two `NSXMLDocument` objects are not considered equal unless they have the same name, same child nodes, same attributes, and so on. The comparison does not consider the parent node (and hence the node’s location). If you want a different standard of comparison, override `isEqual:`.

#### Special Considerations

Because of the architecture and data model of NSXML, when it parses and processes a source of XML it cannot know about your subclass unless you override the class method replacementClass(for:) to return your custom class in place of an `NSXML` class. If your custom class has no direct `NSXML` counterpart—for example, it is a subclass of `NSXMLNode` that represents CDATA sections—then you can walk the tree after it has been created and insert the new node where appropriate.

## Topics

### Initializing NSXMLDocument Objects

convenience init(contentsOf: URL, options: XMLNode.Options) throws

Initializes and returns an NSXMLDocument object created from the XML or HTML contents of a URL-referenced source

init(data: Data, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from an NSData object.

init(rootElement: XMLElement?)

Returns an `NSXMLDocument` object initialized with a single child, the root element.

convenience init(xmlString: String, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from a string containing XML markup text.

class func replacementClass(for: AnyClass) -> AnyClass

Overridden by subclasses to substitute a custom class for an NSXML class that the parser uses to create node instances.

### Managing Document Attributes

var characterEncoding: String?

Sets the character encoding of the receiver to `encoding`,

var documentContentKind: XMLDocument.ContentKind

Sets the kind of output content for the receiver.

var dtd: XMLDTD?

Returns an XMLDTD object representing the internal DTD associated with the receiver.

var isStandalone: Bool

Sets a Boolean value that specifies whether the receiver represents a standalone XML document.

var mimeType: String?

Returns the MIME type for the receiver.

var version: String?

Sets the version of the receiver’s XML.

### Managing the Root Element

func rootElement() -> XMLElement?

Returns the root element of the receiver.

func setRootElement(XMLElement)

Set the root element of the receiver.

### Adding and Removing Child Nodes

func addChild(XMLNode)

Adds a child node after the last of the receiver’s existing children.

func insertChild(XMLNode, at: Int)

Inserts a node object at specified position in the receiver’s array of children.

func insertChildren([XMLNode], at: Int)

Inserts an array of children at a specified position in the receiver’s array of children.

func removeChild(at: Int)

Removes the child node of the receiver located at a specified position in its array of children.

func replaceChild(at: Int, with: XMLNode)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

func setChildren([XMLNode]?)

Sets the child nodes of the receiver.

### Transforming a Document Using XSLT

func object(byApplyingXSLT: Data, arguments: [String : String]?) throws -> Any

Applies the XSLT pattern rules and templates (specified as a data object) to the receiver and returns a document object containing transformed XML or HTML markup.

func object(byApplyingXSLTString: String, arguments: [String : String]?) throws -> Any

Applies the XSLT pattern rules and templates (specified as a string) to the receiver and returns a document object containing transformed XML or HTML markup.

func objectByApplyingXSLT(at: URL, arguments: [String : String]?) throws -> Any

Applies the XSLT pattern rules and templates located at a specified URL to the receiver and returns a document object containing transformed XML markup or an NSData object containing plain text, RTF text, and so on.

### Writing a Document as XML Data

var xmlData: Data

Returns the XML string representation of the receiver—that is, the entire document—encapsulated in a data object.

func xmlData(options: XMLNode.Options) -> Data

Returns the XML string representation of the receiver—that is, the entire document—encapsulated in a data object.

### Validating a Document

func validate() throws

Validates the document against the governing schema and returns whether the document conforms to the schema.

### Constants

Input and Output Options

Input and output options specifically intended for `NSXMLDocument` objects.

enum ContentKind

Type used to define the kind of document content.

Document Content Types

Define document types.

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

class XMLDTD

A representation of a Document Type Definition.

class XMLDTDNode

A representation of element, attribute-list, entity, and notation declarations in a Document Type Definition.

class XMLElement

The element nodes in an XML tree structure.

class XMLNode

The nodes in the abstract, logical tree structure that represents an XML document.

