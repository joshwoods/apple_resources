

- FSKit
- FSItem
- FSItem.SetAttributesRequest
-  consumedAttributes 

Instance Property

# consumedAttributes

The attributes successfully used by the file system.

macOS 15.4+

``` source
var consumedAttributes: FSItem.Attribute { get set }
```

## Discussion

This property is a bit field in Objective-C and an OptionSet in Swift.

## See Also

### Inspecting used attributes

func wasAttributeConsumed(FSItem.Attribute) -> Bool

A method that indicates whether the file system used the given attribute.

struct Attribute

A value that indicates a set of item attributes to get or set.

