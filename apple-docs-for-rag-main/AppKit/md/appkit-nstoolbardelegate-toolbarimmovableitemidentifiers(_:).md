

- AppKit
- NSToolbarDelegate
-  toolbarImmovableItemIdentifiers(\_:) 

Instance Method

# toolbarImmovableItemIdentifiers(\_:)

Asks the delegate to provide the items that people can’t remove from the toolbar or rearrange during the customization process.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+

``` source
@MainActor
optional func toolbarImmovableItemIdentifiers(_ toolbar: NSToolbar) -> Set
```

## Parameters 

`toolbar`  

The toolbar that contains the items.

## Return Value

The set of item identifiers that people can’t remove from the toolbar or move to other locations in the toolbar. Return an empty set to let someone customize all toolbar items.

## Discussion

Implement this method in your delegate and return any items you don’t want people to remove or rearrange. If you don’t implement this method, the toolbar lets people rearrange and remove all toolbar items.

## See Also

### Configuring the behavior of items

func toolbarAllowedItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Asks the delegate to provide the items allowed on the toolbar.

func toolbarDefaultItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Asks the delegate to provide the default items to display on the toolbar.

func toolbarSelectableItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Asks the delegate to provide the set of selectable items in the toolbar.

func toolbar(NSToolbar, itemIdentifier: NSToolbarItem.Identifier, canBeInsertedAt: Int) -> Bool

Asks the delegate for a Boolean value that indicates whether the toolbar can place the item at the specified position.

