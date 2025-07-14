

- FSKit
- FSItem
- FSItem.GetAttributesRequest
-  isAttributeWanted(\_:) 

Instance Method

# isAttributeWanted(\_:)

A method that indicates whether the request wants given attribute.

macOS 15.4+

``` source
func isAttributeWanted(_ attribute: FSItem.Attribute) -> Bool
```

## Parameters 

`attribute`  

The FSItem.Attribute to check.

## See Also

### Inspecting requested attributes

var wantedAttributes: FSItem.Attribute

The attributes requested by the request.

struct Attribute

A value that indicates a set of item attributes to get or set.

