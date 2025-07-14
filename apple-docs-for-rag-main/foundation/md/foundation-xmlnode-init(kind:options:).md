

- Foundation
- XMLNode
-  init(kind:options:) 

Initializer

# init(kind:options:)

Returns an `NSXMLNode` instance initialized with the constant indicating node kind and one or more initialization options.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    kind: XMLNode.Kind,
    options: XMLNode.Options = []
)
```

## Parameters 

`kind`  

An `enum` constant of type XMLNode.Kind that indicates the type of node. See Constants for a list of valid NSXMLNodeKind constants.

`options`  

One or more constants that specify initialization options; if there are multiple constants, bit-OR them together. These options request operations on the represented XML related to fidelity (for example, preserving entities), quoting style, handling of empty elements, and other things. See Constants for a list of valid node-initialization constants.

## Return Value

An `NSXMLNode` object initialized with the given kind and options, or `nil` if the object couldn’t be created. If `kind` is not a valid NSXMLNodeKind constant, the method returns an `NSXMLNode` object of kind `NSXMLInvalidKind`.

## Discussion

Do not use this initializer for creating instances of XMLDTDNode for attribute-list declarations. Instead, use the dtdNode(withXMLString:) class method of this class or the init(xmlString:) method of the `NSXMLDTDNode` class.

## See Also

### Creating and Initializing Node Objects

convenience init(kind: XMLNode.Kind)

Returns an `NSXMLNode` instance initialized with the constant indicating node kind.

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

