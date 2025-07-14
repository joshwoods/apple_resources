

- Foundation
- XMLElement
-  namespaces 

Instance Property

# namespaces

Sets all of the namespace nodes of the receiver at once, replacing any existing namespace nodes.

Mac Catalyst 13.0+macOS 10.0+

``` source
var namespaces: [XMLNode]? { get set }
```

## Parameters 

`namespaces`  

An array of XMLNode objects of kind XMLNode.Kind.namespace. If there are namespace nodes with the same prefix, the first attribute with that prefix is used. Send this message with `namespaces` as `nil` to remove all namespace nodes.

## See Also

### Handling Namespaces

func addNamespace(XMLNode)

Adds a namespace node to the receiver.

func namespace(forPrefix: String) -> XMLNode?

Returns the namespace node with a specified prefix.

func removeNamespace(forPrefix: String)

Removes a namespace node that is identified by a given prefix.

func resolveNamespace(forName: String) -> XMLNode?

Returns the namespace node with the prefix matching the given qualified name.

func resolvePrefix(forNamespaceURI: String) -> String?

Returns the prefix associated with the specified URI.

