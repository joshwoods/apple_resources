

- AppKit
- NSToolbarDelegate
-  toolbarDefaultItemIdentifiers(\_:) 

Instance Method

# toolbarDefaultItemIdentifiers(\_:)

Asks the delegate to provide the default items to display on the toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
optional func toolbarDefaultItemIdentifiers(_ toolbar: NSToolbar) -> [NSToolbarItem.Identifier]
```

## Parameters 

`toolbar`  

The toolbar whose default item identifiers are to be returned.

## Return Value

An array of toolbar item identifiers, each of which represents an item that appears in the default toolbar. Arrange the identifiers in the order you want them to appear in the toolbar, with the first item appearing on the toolbar’s leading edge.

## Discussion

The toolbar calls this method when user settings don’t contain any custom configuration data for the toolbar. The toolbar also calls it to initialize the customization palette’s contents.

Important

Even though this is an optional method, you must implement it if you create the toolbar programatically. If you configure your toolbar in Interface Builder, the configuration there provides the default items.

## See Also

### Configuring the behavior of items

func toolbarAllowedItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Asks the delegate to provide the items allowed on the toolbar.

func toolbarImmovableItemIdentifiers(NSToolbar) -> Set&lt;NSToolbarItem.Identifier>

Asks the delegate to provide the items that people can’t remove from the toolbar or rearrange during the customization process.

func toolbarSelectableItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Asks the delegate to provide the set of selectable items in the toolbar.

func toolbar(NSToolbar, itemIdentifier: NSToolbarItem.Identifier, canBeInsertedAt: Int) -> Bool

Asks the delegate for a Boolean value that indicates whether the toolbar can place the item at the specified position.

