

- Foundation
- XMLNode
-  element(withName:stringValue:) 

Type Method

# element(withName:stringValue:)

Returns an XMLElement object with a single text-node child containing the specified text.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func element(
    withName name: String,
    stringValue string: String
) -> Any
```

## Parameters 

`name`  

A string that is the name (tag identifier) of the element.

`string`  

A string that is the content of the receiver’s text node.

## Return Value

An `NSXMLElement` object with a single text-node child—an `NSXMLNode` object of kind XMLNode.Kind.text—containing the text specified in `string`. Returns `nil` if the object couldn’t be created.

## Discussion

The equivalent XML markup is ``` ``string`` ```.

## See Also

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

