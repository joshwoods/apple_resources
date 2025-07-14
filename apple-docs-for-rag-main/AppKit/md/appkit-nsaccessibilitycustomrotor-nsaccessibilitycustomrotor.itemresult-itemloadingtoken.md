

- AppKit
- NSAccessibilityCustomRotor
- NSAccessibilityCustomRotor.ItemResult
-  itemLoadingToken 

Instance Property

# itemLoadingToken

A token to determine which item to return.

macOS 10.13+

``` source
var itemLoadingToken: NSAccessibilityLoadingToken? { get }
```

## See Also

### Identifying an Item Result

var targetElement: (any NSAccessibilityElementProtocol)?

A target element that references an element to message for accessibility properties.

var targetRange: NSRange

A range that specifies the area of interest for text-based elements.

var customLabel: String?

A localized label to use instead of the default item label to describe the item result.

