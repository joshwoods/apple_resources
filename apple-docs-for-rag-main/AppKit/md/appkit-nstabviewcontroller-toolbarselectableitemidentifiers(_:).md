

- AppKit
- NSTabViewController
-  toolbarSelectableItemIdentifiers(\_:) 

Instance Method

# toolbarSelectableItemIdentifiers(\_:)

Returns the array of identifier strings for the selectable toolbar items

macOS 10.10+

``` source
@MainActor
func toolbarSelectableItemIdentifiers(_ toolbar: NSToolbar) -> [NSToolbarItem.Identifier]
```

## Parameters 

`toolbar`  

The toolbar making the request.

## Return Value

An array of NSString objects, each of which contains an identifier for a toolbar item that may be selected.

## Discussion

This method is called for tab view interfaces that use the NSTabViewController.TabStyle.toolbar style. Use this method to indicate which toolbar items are selectable. When an item is selected, the toolbar displays it with a visual highlight and updates the selectedTabViewItemIndex property. Typically, the toolbar items associated with tabs are selectable so that the user can tell which tab is selected.

If you override this method, you must call `super` at some point in your implementation. The default implementation of this method returns the identifiers for all toolbar items that correspond to tabs in the tab bar interface.

## See Also

### Responding to Toolbar Events

func toolbar(NSToolbar, itemForItemIdentifier: NSToolbarItem.Identifier, willBeInsertedIntoToolbar: Bool) -> NSToolbarItem?

Returns the toolbar item for the specified identifier.

func toolbarAllowedItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Returns the array of identifier strings for the allowed toolbar items.

func toolbarDefaultItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Returns the array of identifier strings for the default toolbar items.

