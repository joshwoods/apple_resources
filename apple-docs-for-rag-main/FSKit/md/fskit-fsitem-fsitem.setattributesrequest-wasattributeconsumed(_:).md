

- FSKit
- FSItem
- FSItem.SetAttributesRequest
-  wasAttributeConsumed(\_:) 

Instance Method

# wasAttributeConsumed(\_:)

A method that indicates whether the file system used the given attribute.

macOS 15.4+

``` source
func wasAttributeConsumed(_ attribute: FSItem.Attribute) -> Bool
```

## Parameters 

`attribute`  

The FSItem.Attribute to check.

## See Also

### Inspecting used attributes

var consumedAttributes: FSItem.Attribute

The attributes successfully used by the file system.

struct Attribute

A value that indicates a set of item attributes to get or set.

