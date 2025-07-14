

- Foundation
- XMLElement
-  elements(forLocalName:uri:) 

Instance Method

# elements(forLocalName:uri:)

Returns the child element nodes (as `NSXMLElement` objects) of the receiver that are matched with the specified local name and URI.

Mac Catalyst 13.0+macOS 10.0+

``` source
func elements(
    forLocalName localName: String,
    uri URI: String?
) -> [XMLElement]
```

## Parameters 

`localName`  

A string specifying a local name of an element.

`URI`  

A string specifying a URI associated with an element.

## Return Value

An array of `NSXMLElement` objects or an empty array if no matching children could be found.

## See Also

### Obtaining Child Elements

func elements(forName: String) -> [XMLElement]

Returns the child element nodes (as `NSXMLElement` objects) of the receiver that have a specified name.

