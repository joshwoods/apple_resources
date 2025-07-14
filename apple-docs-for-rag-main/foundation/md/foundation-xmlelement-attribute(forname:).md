

- Foundation
- XMLElement
-  attribute(forName:) 

Instance Method

# attribute(forName:)

Returns the attribute node of the receiver with the specified name.

Mac Catalyst 13.0+macOS 10.0+

``` source
func attribute(forName name: String) -> XMLNode?
```

## Parameters 

`name`  

A string specifying the name of an attribute.

## Return Value

An XML node object representing a matching attribute or `nil` if no such node was found.

## Discussion

If `name` is a qualified name, then this method invokes attribute(forLocalName:uri:) with the URI parameter set to the URI associated with the prefix. Otherwise comparison is based on string equality of the qualified or non-qualified name.

## See Also

### Handling Attributes

func addAttribute(XMLNode)

Adds an attribute node to the receiver.

func attribute(forLocalName: String, uri: String?) -> XMLNode?

Returns the attribute node of the receiver that is identified by a local name and URI.

var attributes: [XMLNode]?

Sets all attributes of the receiver at once, replacing any existing attribute nodes.

func removeAttribute(forName: String)

Removes an attribute node identified by name.

func setAttributesWith([String : String])

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

