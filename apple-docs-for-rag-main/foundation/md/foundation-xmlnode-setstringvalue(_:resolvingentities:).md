

- Foundation
- XMLNode
-  setStringValue(\_:resolvingEntities:) 

Instance Method

# setStringValue(\_:resolvingEntities:)

Sets the content of the receiver as a string value and, optionally, resolves character references, predefined entities, and user-defined entities as declared in the associated DTD.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setStringValue(
    _ string: String,
    resolvingEntities resolve: Bool
)
```

## Parameters 

`string`  

A string to assign as the value of the receiver.

`resolve`  

true to resolve character references, predefined entities, and user-defined entities as declared in the associated DTD; false otherwise. Namespace and processing-instruction nodes have their entities resolved even if `resolve` is false.

## Discussion

User-defined entities not declared in the DTD remain in their unresolved form. This method can only be invoked on `NSXMLNode` objects that may have content, specifically elements, attributes, namespaces, processing instructions, text, and DTD-declaration nodes. Setting the string value of a node object removes all existing children, including processing instructions and comments. Setting the string value of an element -node object creates a text node as the sole child.

## See Also

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

var uri: String?

Returns the URI associated with the receiver.

