

- Foundation
- XMLElement
-  namespace(forPrefix:) 

Instance Method

# namespace(forPrefix:)

Returns the namespace node with a specified prefix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func namespace(forPrefix name: String) -> XMLNode?
```

## Parameters 

`name`  

A string specifying a namespace prefix.

## Return Value

An XMLNode object of kind XMLNode.Kind.namespace or `nil` if there is no namespace node with that prefix.

## See Also

### Handling Namespaces

func addNamespace(XMLNode)

Adds a namespace node to the receiver.

var namespaces: [XMLNode]?

Sets all of the namespace nodes of the receiver at once, replacing any existing namespace nodes.

func removeNamespace(forPrefix: String)

Removes a namespace node that is identified by a given prefix.

func resolveNamespace(forName: String) -> XMLNode?

Returns the namespace node with the prefix matching the given qualified name.

func resolvePrefix(forNamespaceURI: String) -> String?

Returns the prefix associated with the specified URI.

