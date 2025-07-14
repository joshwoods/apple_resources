

- WebKit
- WebHistory
-  addItems(\_:) Deprecated

Instance Method

# addItems(\_:)

Inserts or updates the specified items in the web history.

macOS 10.3–10.14Deprecated

``` source
func addItems(_ newItems: [Any]!)
```

## Parameters 

`newItems`  

An array of web history items to add. If an item in the array already exists in the web history this method replaces the existing item, so that the last-visited date for the item is updated.

## Discussion

When successful, this method posts a notification (WebHistoryItemsAddedNotification).

## See Also

### Adding and Removing History Items

func removeItems([Any]!)

Removes the specified items from the web history.

Deprecated

func removeAllItems()

Removes all items from the web history.

Deprecated

