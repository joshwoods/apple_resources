

- Foundation
- XMLNode
-  uri 

Instance Property

# uri

Returns the URI associated with the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var uri: String? { get set }
```

## Discussion

A node’s URI is derived from its namespace or a document’s URI; for documents, the URI comes either from the parsed XML or is explicitly set. You cannot change the URI for a particular node other for than a namespace or document node.

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

func setStringValue(String, resolvingEntities: Bool)

Sets the content of the receiver as a string value and, optionally, resolves character references, predefined entities, and user-defined entities as declared in the associated DTD.

