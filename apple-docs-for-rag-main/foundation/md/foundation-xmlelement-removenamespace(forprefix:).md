

- Foundation
- XMLElement
-  removeNamespace(forPrefix:) 

Instance Method

# removeNamespace(forPrefix:)

Removes a namespace node that is identified by a given prefix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeNamespace(forPrefix name: String)
```

## Parameters 

`name`  

A string that is the prefix for a namespace.

## Discussion

The removed XML node object is removed.

## See Also

### Handling Namespaces

func addNamespace(XMLNode)

Adds a namespace node to the receiver.

var namespaces: [XMLNode]?

Sets all of the namespace nodes of the receiver at once, replacing any existing namespace nodes.

func namespace(forPrefix: String) -> XMLNode?

Returns the namespace node with a specified prefix.

func resolveNamespace(forName: String) -> XMLNode?

Returns the namespace node with the prefix matching the given qualified name.

func resolvePrefix(forNamespaceURI: String) -> String?

Returns the prefix associated with the specified URI.

