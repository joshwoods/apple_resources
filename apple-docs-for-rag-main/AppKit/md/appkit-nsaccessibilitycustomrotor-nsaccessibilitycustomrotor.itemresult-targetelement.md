

- AppKit
- NSAccessibilityCustomRotor
- NSAccessibilityCustomRotor.ItemResult
-  targetElement 

Instance Property

# targetElement

A target element that references an element to message for accessibility properties.

macOS 10.13+

``` source
weak var targetElement: (any NSAccessibilityElementProtocol)? { get }
```

## See Also

### Identifying an Item Result

var itemLoadingToken: NSAccessibilityLoadingToken?

A token to determine which item to return.

var targetRange: NSRange

A range that specifies the area of interest for text-based elements.

var customLabel: String?

A localized label to use instead of the default item label to describe the item result.

