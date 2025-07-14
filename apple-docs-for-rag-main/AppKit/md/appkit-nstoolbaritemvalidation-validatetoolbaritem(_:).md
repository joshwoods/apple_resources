

- AppKit
- NSToolbarItemValidation
-  validateToolbarItem(\_:) 

Instance Method

# validateToolbarItem(\_:)

If this method is implemented and returns false, NSToolbar will disable `theItem`; returning true causes `theItem` to be enabled.

macOS

``` source
@MainActor
func validateToolbarItem(_ item: NSToolbarItem) -> Bool
```

**Required**

## Discussion

NSToolbar only calls this method for image items.

Note

validateToolbarItem: is called very frequently, so it must be efficient.

If the receiver is the `target` for the actions of multiple toolbar items, it’s necessary to determine which toolbar item `theItem` refers to by testing the `itemIdentifier`.

```
-(BOOL)validateToolbarItem:(NSToolbarItem *)toolbarItem
{
    BOOL enable = NO;
    if ([[toolbarItem itemIdentifier] isEqual:SaveDocToolbarItemIdentifier]) {
        // We will return YES (enable the save item)
        // only when the document is dirty and needs saving
        enable = [self isDocumentEdited];
    } else if ([[toolbarItem itemIdentifier] isEqual:NSToolbarPrintItemIdentifier]) {
        // always enable print for this window
        enable = YES;
    }
    return enable;
}
```

## See Also

### Related Documentation

func validateVisibleItems()

Validates the toolbar’s visible items during a window update.

var action: Selector?

The action method to call when someone clicks on the toolbar item.

var target: AnyObject?

The object that defines the action method the toolbar item calls when clicked.

Toolbar Programming Topics for Cocoa

func validate()

Validates the toolbar item’s menu and its ability to perfrom its action.

