

- Foundation
- XMLElement
-  addNamespace(\_:) 

Instance Method

# addNamespace(\_:)

Adds a namespace node to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addNamespace(_ aNamespace: XMLNode)
```

## Parameters 

`aNamespace`  

An XML node object of kind XMLNode.Kind.namespace. If the receiver already has a namespace with the same name, `aNamespace` is not added.

## See Also

### Handling Namespaces

var namespaces: [XMLNode]?

Sets all of the namespace nodes of the receiver at once, replacing any existing namespace nodes.

func namespace(forPrefix: String) -> XMLNode?

Returns the namespace node with a specified prefix.

func removeNamespace(forPrefix: String)

Removes a namespace node that is identified by a given prefix.

func resolveNamespace(forName: String) -> XMLNode?

Returns the namespace node with the prefix matching the given qualified name.

func resolvePrefix(forNamespaceURI: String) -> String?

Returns the prefix associated with the specified URI.

