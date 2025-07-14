

- Foundation
- XMLElement
-  removeAttribute(forName:) 

Instance Method

# removeAttribute(forName:)

Removes an attribute node identified by name.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeAttribute(forName name: String)
```

## Parameters 

`name`  

A string specifying the name of an attribute.

## See Also

### Handling Attributes

func addAttribute(XMLNode)

Adds an attribute node to the receiver.

func attribute(forName: String) -> XMLNode?

Returns the attribute node of the receiver with the specified name.

func attribute(forLocalName: String, uri: String?) -> XMLNode?

Returns the attribute node of the receiver that is identified by a local name and URI.

var attributes: [XMLNode]?

Sets all attributes of the receiver at once, replacing any existing attribute nodes.

func setAttributesWith([String : String])

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

