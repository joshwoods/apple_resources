

- Foundation
- XMLNode
-  predefinedNamespace(forPrefix:) 

Type Method

# predefinedNamespace(forPrefix:)

Returns an `NSXMLNode` object representing one of the predefined namespaces with the specified prefix.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func predefinedNamespace(forPrefix name: String) -> XMLNode?
```

## Parameters 

`name`  

A string specifying a prefix for a predefined namespace, for example “xml”, “xs”, or “xsi”.

## Return Value

An `NSXMLNode` object of kind XMLNode.Kind.namespace or `nil` if the object couldn’t be created. If something other than a predefined-namespace prefix is specified, the method returns `nil`.

## See Also

### Related Documentation

class func prefix(forName: String) -> String?

Returns the prefix from the specified qualified name.

class func localName(forName: String) -> String

Returns the local name from the specified qualified name.

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

class func processingInstruction(withName: String, stringValue: String) -> Any

Returns an `NSXMLNode` object representing a processing instruction with a specified name and value.

