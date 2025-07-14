

- FSKit
- FSItem
- FSItem.GetAttributesRequest
-  wantedAttributes 

Instance Property

# wantedAttributes

The attributes requested by the request.

macOS 15.4+

``` source
var wantedAttributes: FSItem.Attribute { get set }
```

## Discussion

This property is a bit field in Objective-C and an OptionSet in Swift.

## See Also

### Inspecting requested attributes

func isAttributeWanted(FSItem.Attribute) -> Bool

A method that indicates whether the request wants given attribute.

struct Attribute

A value that indicates a set of item attributes to get or set.

