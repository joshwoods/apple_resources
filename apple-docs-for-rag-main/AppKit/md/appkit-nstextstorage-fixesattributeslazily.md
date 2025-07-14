

- AppKit
- NSTextStorage
-  fixesAttributesLazily 

Instance Property

# fixesAttributesLazily

A Boolean value that indicates whether the text storage object fixes attributes lazily.

macOS 10.0+

``` source
var fixesAttributesLazily: Bool { get }
```

## Discussion

When subclassing, the default value of this property is false, meaning that your subclass fixes attributes immediately when they change. The system’s concrete subclass overrides this property and sets it to true.

## See Also

### Fixing the string attributes

func invalidateAttributes(in: NSRange)

Invalidates attributes in the specified range.

func ensureAttributesAreFixed(in: NSRange)

Ensures that attribute fixing occurs in the specified range.

