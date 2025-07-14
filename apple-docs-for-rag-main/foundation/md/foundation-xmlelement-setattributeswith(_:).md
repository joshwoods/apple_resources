

- Foundation
- XMLElement
-  setAttributesWith(\_:) 

Instance Method

# setAttributesWith(\_:)

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setAttributesWith(_ attributes: [String : String])
```

## Parameters 

`attributes`  

A dictionary of key-value pairs where the attribute name is the key and the object value of the attribute is the dictionary value.

## Discussion

The method uses these names and object values to create XMLNode objects of kind XMLNode.Kind.attribute. Existing attributes are removed.

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

func removeAttribute(forName: String)

Removes an attribute node identified by name.

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

