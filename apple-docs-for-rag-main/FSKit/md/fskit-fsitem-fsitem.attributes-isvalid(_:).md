

- FSKit
- FSItem
- FSItem.Attributes
-  isValid(\_:) 

Instance Method

# isValid(\_:)

Returns a Boolean value that indicates whether the attribute is valid.

macOS 15.4+

``` source
func isValid(_ attribute: FSItem.Attribute) -> Bool
```

## Discussion

If the value returned by this method is `YES` (Objective-C) or `true` (Swift), a caller can safely use the given attribute.

## See Also

### Validating and invalidating attributes

func invalidateAllProperties()

Marks all attributes inactive.

