

- AppKit
- NSToolbarItem
- NSToolbarItem.VisibilityPriority
-  low 

Type Property

# low

The lowest-priority for a toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
static let low: NSToolbarItem.VisibilityPriority
```

## Discussion

The toolbar pushes items with this priority to the overflow menu first, even before items with the standard priority.

## See Also

### Visibility priorities

static let standard: NSToolbarItem.VisibilityPriority

The default visibility priority.

static let high: NSToolbarItem.VisibilityPriority

A high priority that makes it less likely for the toolbar item to move to the overflow item.

static let user: NSToolbarItem.VisibilityPriority

The highest priority for items in the toolbar.

