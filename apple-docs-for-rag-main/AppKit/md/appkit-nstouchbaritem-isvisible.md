

- AppKit
- NSTouchBarItem
-  isVisible 

Instance Property

# isVisible

A Boolean value that reflects whether or not the item is visible.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var isVisible: Bool { get }
```

## Discussion

When true, this item is shown in a currently visible bar. This property is always false for spaces, proxy items, and groups.

This property is key-value observable.

## See Also

### Managing item visibility

var visibilityPriority: NSTouchBarItem.Priority

Determines which items are shown in a bar when space is limited.

struct Priority

Priorities for the visibility of a Touch Bar item.

