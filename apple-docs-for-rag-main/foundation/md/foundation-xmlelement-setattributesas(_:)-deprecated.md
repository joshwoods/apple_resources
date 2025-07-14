

- Foundation
- XMLElement
-  setAttributesAs(\_:) Deprecated

Instance Method

# setAttributesAs(\_:)

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4Deprecated

``` source
func setAttributesAs(_ attributes: [AnyHashable : Any])
```

Deprecated

This method is deprecated because it does not function properly. Instead use setAttributesWith(_:).

## Parameters 

`attributes`  

A dictionary of key-value pairs where the attribute name is the key and the object value of the attribute is the dictionary value.

## Discussion

The method uses these names and object values to create XMLNode objects of kind XMLNode.Kind.attribute. Existing attributes are not removed.

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

func setAttributesWith([String : String])

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

