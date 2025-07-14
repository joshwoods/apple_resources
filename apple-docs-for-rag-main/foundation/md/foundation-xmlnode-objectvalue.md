

- Foundation
- XMLNode
-  objectValue 

Instance Property

# objectValue

Returns the object value of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var objectValue: Any? { get set }
```

## Return Value

The object value of the receiver, which may be the same as the value returned by stringValue. For nodes without content (for example, document nodes), this method returns the string value, or an empty string if there is no string value.

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

var stringValue: String?

Returns the content of the receiver as a string value.

func setStringValue(String, resolvingEntities: Bool)

Sets the content of the receiver as a string value and, optionally, resolves character references, predefined entities, and user-defined entities as declared in the associated DTD.

var uri: String?

Returns the URI associated with the receiver.

