

- AppKit
- NSAccessibilityCustomRotor
- NSAccessibilityCustomRotor.SearchParameters
-  currentItem 

Instance Property

# currentItem

The current item that determines where the search starts.

macOS 10.13+

``` source
var currentItem: NSAccessibilityCustomRotor.ItemResult? { get set }
```

## Discussion

If this value is `nil`, searchDirection determines the current item. A search direction of NSAccessibilityCustomRotor.SearchDirection.next begins the search from the first item, and a search direction of NSAccessibilityCustomRotor.SearchDirection.previous begins the search from the last item.

## See Also

### Managing the Current Item

class ItemResult

A target accessibility element that a custom rotor references.

