

- AppKit
- NSToolbarDelegate
-  toolbarDidRemoveItem(\_:) 

Instance Method

# toolbarDidRemoveItem(\_:)

Tells the delegate that the toolbar removed the specified item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
optional func toolbarDidRemoveItem(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didRemoveItemNotification.

## Discussion

Use this method to update data structures related to your toolbar items.

## See Also

### Adding and removing items

func toolbar(NSToolbar, itemForItemIdentifier: NSToolbarItem.Identifier, willBeInsertedIntoToolbar: Bool) -> NSToolbarItem?

Asks the delegate for the toolbar item associated with the specified identifier.

func toolbarWillAddItem(Notification)

Tells the delegate that the toolbar is about to add the specified item.

typealias Identifier

A string value that you use to differentiate your app’s toolbars.

