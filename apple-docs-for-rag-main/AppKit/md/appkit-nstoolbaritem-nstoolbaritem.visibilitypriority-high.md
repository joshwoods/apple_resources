

- AppKit
- NSToolbarItem
- NSToolbarItem.VisibilityPriority
-  high 

Type Property

# high

A high priority that makes it less likely for the toolbar item to move to the overflow item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
static let high: NSToolbarItem.VisibilityPriority
```

## Discussion

The toolbar moves items with standard priority to the overflow menu before it moves items with this priority.

## See Also

### Visibility priorities

static let standard: NSToolbarItem.VisibilityPriority

The default visibility priority.

static let low: NSToolbarItem.VisibilityPriority

The lowest-priority for a toolbar item.

static let user: NSToolbarItem.VisibilityPriority

The highest priority for items in the toolbar.

