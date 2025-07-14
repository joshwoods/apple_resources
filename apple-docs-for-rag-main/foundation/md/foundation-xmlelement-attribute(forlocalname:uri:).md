

- Foundation
- XMLElement
-  attribute(forLocalName:uri:) 

Instance Method

# attribute(forLocalName:uri:)

Returns the attribute node of the receiver that is identified by a local name and URI.

Mac Catalyst 13.0+macOS 10.0+

``` source
func attribute(
    forLocalName localName: String,
    uri URI: String?
) -> XMLNode?
```

## Parameters 

`localName`  

A string specifying the local name of an attribute.

`URI`  

A sting identifying the URI associated with an attribute.

## Return Value

An XML node object representing a matching attribute or `nil` if no such node was found.

## See Also

### Handling Attributes

func addAttribute(XMLNode)

Adds an attribute node to the receiver.

func attribute(forName: String) -> XMLNode?

Returns the attribute node of the receiver with the specified name.

var attributes: [XMLNode]?

Sets all attributes of the receiver at once, replacing any existing attribute nodes.

func removeAttribute(forName: String)

Removes an attribute node identified by name.

func setAttributesWith([String : String])

Sets the attributes of the receiver based on the key-value pairs specified in the passed dictionary.

func setAttributesAs([AnyHashable : Any])

Sets the attributes of the receiver based on the key-value pairs specified in the passed-in dictionary.

Deprecated

