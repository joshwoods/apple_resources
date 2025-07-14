

- UIKit
- UIFocusItem
-  focusGroupPriority 

Instance Property

# focusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
optional var focusGroupPriority: UIFocusGroupPriority { get }
```

## Discussion

The system automatically assigns each focusable item in a focus group one of the predefined system priorities. The system assigns the currentlyFocused priority to the focused item, previouslyFocused to the group’s previous focused item, and ignored for all other items. The visible item with the highest priority is the group’s primary item.

You can override the default priority of an item to customize the primary item of a group. When setting a custom priority, you can only increase the item’s priority above its system-provided value, not decrease it. The system-provided priority is always the minimum priority applied for the item. The system ignores any priority lower than `0`.

## See Also

### Determining the focus priority

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

