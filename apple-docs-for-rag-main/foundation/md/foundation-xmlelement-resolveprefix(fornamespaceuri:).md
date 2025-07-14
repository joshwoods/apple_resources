

- Foundation
- XMLElement
-  resolvePrefix(forNamespaceURI:) 

Instance Method

# resolvePrefix(forNamespaceURI:)

Returns the prefix associated with the specified URI.

Mac Catalyst 13.0+macOS 10.0+

``` source
func resolvePrefix(forNamespaceURI namespaceURI: String) -> String?
```

## Parameters 

`namespaceURI`  

A string identifying the URI associated with the namespace.

## Return Value

A string that is the matching prefix or `nil` if it finds no matching prefix.

## Discussion

The method looks in the entire namespace chain for the URI.

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

func resolveNamespace(forName: String) -> XMLNode?

Returns the namespace node with the prefix matching the given qualified name.

