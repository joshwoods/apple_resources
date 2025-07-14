

- Foundation
- XMLNode
-  kind 

Instance Property

# kind

Returns the kind of node the receiver is as a constant of type XMLNode.Kind.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kind: XMLNode.Kind { get }
```

## Discussion

`NSXMLNode` objects can represent documents, elements, attributes, namespaces, text, processing instructions, comments, document type declarations, and specific declarations within DTDs. See Constants for a list of valid NSXMLNodeKind constants

## See Also

### Related Documentation

convenience init(kind: XMLNode.Kind)

Returns an `NSXMLNode` instance initialized with the constant indicating node kind.

### Managing XML Node Objects

var index: Int

Returns the index of the receiver identifying its position relative to its sibling nodes.

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

