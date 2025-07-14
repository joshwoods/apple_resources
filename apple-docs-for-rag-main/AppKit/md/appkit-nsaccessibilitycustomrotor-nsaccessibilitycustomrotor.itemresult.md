

- AppKit
- NSAccessibilityCustomRotor
-  NSAccessibilityCustomRotor.ItemResult 

Class

# NSAccessibilityCustomRotor.ItemResult

A target accessibility element that a custom rotor references.

macOS 10.13+

``` source
class ItemResult
```

## Topics

### Creating an Item Result

init(targetElement: any NSAccessibilityElementProtocol)

Creates an item result with the specified target element.

init(itemLoadingToken: NSAccessibilityLoadingToken, customLabel: String)

Creates an item result with the specified item load token and custom label.

### Identifying an Item Result

var targetElement: (any NSAccessibilityElementProtocol)?

A target element that references an element to message for accessibility properties.

var itemLoadingToken: NSAccessibilityLoadingToken?

A token to determine which item to return.

var targetRange: NSRange

A range that specifies the area of interest for text-based elements.

var customLabel: String?

A localized label to use instead of the default item label to describe the item result.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing the Current Item

var currentItem: NSAccessibilityCustomRotor.ItemResult?

The current item that determines where the search starts.

