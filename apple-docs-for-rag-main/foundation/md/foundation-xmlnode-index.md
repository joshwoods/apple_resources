

- Foundation
- XMLNode
-  index 

Instance Property

# index

Returns the index of the receiver identifying its position relative to its sibling nodes.

Mac Catalyst 13.0+macOS 10.0+

``` source
var index: Int { get }
```

## Return Value

An integer that is the index of the receiver relative to its sibling nodes.

## Discussion

The first child node of a parent has an index of zero.

## See Also

### Related Documentation

func child(at: Int) -> XMLNode?

Returns the child node of the receiver at the specified location.

### Managing XML Node Objects

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

