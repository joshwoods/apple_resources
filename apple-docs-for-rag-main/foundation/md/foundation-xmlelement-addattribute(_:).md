

- Foundation
- XMLElement
-  addAttribute(\_:) 

Instance Method

# addAttribute(\_:)

Adds an attribute node to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addAttribute(_ attribute: XMLNode)
```

## Parameters 

`attribute`  

An XML node object representing an attribute. If the receiver already has an attribute with the same name, `anAttribute` replaces the old attribute.

## Discussion

The order of multiple attributes is preserved if the `NSXMLPreserveAttributeOrder` option is specified when the element is created.

## See Also

### Handling Attributes

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

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

