

- AppKit
- NSTextStorage
-  ensureAttributesAreFixed(in:) 

Instance Method

# ensureAttributesAreFixed(in:)

Ensures that attribute fixing occurs in the specified range.

macOS 10.0+

``` source
func ensureAttributesAreFixed(in range: NSRange)
```

## Parameters 

`range`  

The range of characters to examine.

## Discussion

An `NSTextStorage` object using lazy attribute fixing is required to call this method before accessing any attributes within `range`. This method gives attribute fixing a chance to occur if necessary. `NSTextStorage` subclasses wishing to support laziness must call this method from all attribute accessors they implement.

## See Also

### Fixing the string attributes

func invalidateAttributes(in: NSRange)

Invalidates attributes in the specified range.

var fixesAttributesLazily: Bool

A Boolean value that indicates whether the text storage object fixes attributes lazily.

