

- AppKit
- NSToolbarItem
- NSToolbarItem.VisibilityPriority
-  user 

Type Property

# user

The highest priority for items in the toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
static let user: NSToolbarItem.VisibilityPriority
```

## Discussion

The toolbar pushes these items to the overflow menu last.

## See Also

### Visibility priorities

static let standard: NSToolbarItem.VisibilityPriority

The default visibility priority.

static let low: NSToolbarItem.VisibilityPriority

The lowest-priority for a toolbar item.

static let high: NSToolbarItem.VisibilityPriority

A high priority that makes it less likely for the toolbar item to move to the overflow item.

