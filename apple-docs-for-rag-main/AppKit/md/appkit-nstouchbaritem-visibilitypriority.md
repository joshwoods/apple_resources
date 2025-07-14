

- AppKit
- NSTouchBarItem
-  visibilityPriority 

Instance Property

# visibilityPriority

Determines which items are shown in a bar when space is limited.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var visibilityPriority: NSTouchBarItem.Priority { get set }
```

## Discussion

The bar hides items of lower priority when there is not enough space to show all items. Use this property to specify the relative priority of the items in your bar.

## See Also

### Managing item visibility

struct Priority

Priorities for the visibility of a Touch Bar item.

var isVisible: Bool

A Boolean value that reflects whether or not the item is visible.

