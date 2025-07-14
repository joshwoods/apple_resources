

- AppKit
- NSAccessibilityCustomRotor
- NSAccessibilityCustomRotor.ItemResult
-  targetRange 

Instance Property

# targetRange

A range that specifies the area of interest for text-based elements.

macOS 10.13+

``` source
var targetRange: NSRange { get set }
```

## See Also

### Identifying an Item Result

var targetElement: (any NSAccessibilityElementProtocol)?

A target element that references an element to message for accessibility properties.

var itemLoadingToken: NSAccessibilityLoadingToken?

A token to determine which item to return.

var customLabel: String?

A localized label to use instead of the default item label to describe the item result.

