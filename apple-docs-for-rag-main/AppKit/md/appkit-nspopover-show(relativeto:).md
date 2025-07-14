

- AppKit
- NSPopover
-  show(relativeTo:) 

Instance Method

# show(relativeTo:)

Shows the popover anchored to the specified toolbar item.

macOS 14.0+

``` source
@MainActor
func show(relativeTo toolbarItem: NSToolbarItem)
```

## Parameters 

`toolbarItem`  

The toolbar item anchoring the popover.

## Discussion

Use this method to display a popover relative to a toolbar item. When the item is in the overflow menu, the popover presents itself from another appropriate affordance in the window. See show(relativeTo:of:preferredEdge:) for popover behavior.

This method raises an invalidArgumentException if it can’t locate the toolbar item. This could occur if the item isn’t in a toolbar, or because the toolbar isn’t in the window.

