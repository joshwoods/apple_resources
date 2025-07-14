

- UIKit
- UIContextMenuConfiguration
-  badgeCount 

Instance Property

# badgeCount

The number of items in a multiple-item interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var badgeCount: Int { get set }
```

## Discussion

The system uses this value to generate a badge for the stack of selected items to indicate how many items the menu is acting on. A value below `2` hides the badge. If you don’t set this value, the system determines it automatically.

## See Also

### Handling multiple-item interactions

var secondaryItemIdentifiers: Set&lt;AnyHashable>

A set of identifiers corresponding to each item other than the primary item in a multiple-item interaction.

