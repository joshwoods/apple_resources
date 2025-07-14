

- Foundation
- XMLElement
-  attributes 

Instance Property

# attributes

Sets all attributes of the receiver at once, replacing any existing attribute nodes.

Mac Catalyst 13.0+macOS 10.0+

``` source
var attributes: [XMLNode]? { get set }
```

## Parameters 

`attributes`  

An array of XMLNode objects of kind XMLNode.Kind.attribute. If there are attribute nodes with the same name, the first attribute with that name is used. Send this message with `attributes` as `nil` to remove all attributes.

## Discussion

To set attributes in an element node using an NSDictionary object as the input parameter, see setAttributesWith(_:).

## See Also

### Handling Attributes

func addAttribute(XMLNode)

Adds an attribute node to the receiver.

func attribute(forName: String) -> XMLNode?

Returns the attribute node of the receiver with the specified name.

func attribute(forLocalName: String, uri: String?) -> XMLNode?

Returns the attribute node of the receiver that is identified by a local name and URI.

func removeAttribute(forName: String)

Removes an attribute node identified by name.

func setAttributesWith([String : String])

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

