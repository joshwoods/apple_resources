

- Foundation
- XMLElement
-  resolveNamespace(forName:) 

Instance Method

# resolveNamespace(forName:)

Returns the namespace node with the prefix matching the given qualified name.

Mac Catalyst 13.0+macOS 10.0+

``` source
func resolveNamespace(forName name: String) -> XMLNode?
```

## Parameters 

`name`  

A string that is the qualified name for a namespace (a qualified name is prefix plus local name).

## Return Value

An XMLNode object of kind XMLNode.Kind.namespace or `nil` if there is no matching namespace node.

## Discussion

The method looks in the entire namespace chain for the prefix.

## See Also

### Handling Namespaces

func addNamespace(XMLNode)

Adds a namespace node to the receiver.

var namespaces: [XMLNode]?

Sets all of the namespace nodes of the receiver at once, replacing any existing namespace nodes.

func namespace(forPrefix: String) -> XMLNode?

Returns the namespace node with a specified prefix.

func removeNamespace(forPrefix: String)

Removes a namespace node that is identified by a given prefix.

func resolvePrefix(forNamespaceURI: String) -> String?

Returns the prefix associated with the specified URI.

