

- Foundation
- XMLNode
-  level 

Instance Property

# level

Returns the nesting level of the receiver within the tree hierarchy.

Mac Catalyst 13.0+macOS 10.0+

``` source
var level: Int { get }
```

## Return Value

An integer indicating a nesting level.

## Discussion

The root element of a document has a nesting level of one.

## See Also

### Managing XML Node Objects

var index: Int

Returns the index of the receiver identifying its position relative to its sibling nodes.

var kind: XMLNode.Kind

Returns the kind of node the receiver is as a constant of type XMLNode.Kind.

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

