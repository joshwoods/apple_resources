

- Foundation
- XMLNode
-  name 

Instance Property

# name

Returns the name of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var name: String? { get set }
```

## Return Value

Returns a string specifying the name of the receiver. May return `nil` if the receiver is not a valid kind of node (see discussion).

## Discussion

This method is applicable only to `NSXMLNode` objects representing elements, attributes, namespaces, processing instructions, and DTD-declaration nodes. If the receiver is not an object of one of these kinds, this method returns `nil`. For example, in the following construction:

```
Chapter One
```

The returned name for the element is “title”. If the name is associated with a namespace, the qualified name is returned. For example, if you create an element with local name “foo” and URI “http://bar.com” and the namespace “xmlns:baz=‘http://bar.com’” is applied to this node, when you invoke this method on the node you get “baz:foo”.

## See Also

### Managing XML Node Objects

var index: Int

Returns the index of the receiver identifying its position relative to its sibling nodes.

var kind: XMLNode.Kind

Returns the kind of node the receiver is as a constant of type XMLNode.Kind.

var level: Int

Returns the nesting level of the receiver within the tree hierarchy.

var objectValue: Any?

Returns the object value of the receiver.

var stringValue: String?

Returns the content of the receiver as a string value.

func setStringValue(String, resolvingEntities: Bool)

Sets the content of the receiver as a string value and, optionally, resolves character references, predefined entities, and user-defined entities as declared in the associated DTD.

var uri: String?

Returns the URI associated with the receiver.

