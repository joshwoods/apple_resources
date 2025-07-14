

- AppKit
- NSUserInterfaceItemSearching
-  performAction(forItem:) 

Instance Method

# performAction(forItem:)

Invoked when the user selects a search result in Help menu.

macOS

``` source
optional func performAction(forItem item: Any)
```

## Parameters 

`item`  

An item in the help menu.

## Discussion

The default implementation brings up Help Viewer for a Help item.

## See Also

### Search Help Content

func searchForItems(withSearch: String, resultLimit: Int, matchedItemHandler: ([Any]) -> Void)

Search for the specified items, with the result limit.

**Required**

