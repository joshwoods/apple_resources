

- AppKit
- NSTextStorage
-  invalidateAttributes(in:) 

Instance Method

# invalidateAttributes(in:)

Invalidates attributes in the specified range.

macOS 10.0+

``` source
func invalidateAttributes(in range: NSRange)
```

## Parameters 

`range`  

The range of characters whose attributes the method should invalidate.

## Discussion

Called from processEditing() to invalidate attributes when the text storage changes. If the receiver isn’t lazy, this method calls fixAttributes(in:). If lazy attribute fixing is in effect, this method instead records the range needing fixing.

## See Also

### Fixing the string attributes

func ensureAttributesAreFixed(in: NSRange)

Ensures that attribute fixing occurs in the specified range.

var fixesAttributesLazily: Bool

A Boolean value that indicates whether the text storage object fixes attributes lazily.

