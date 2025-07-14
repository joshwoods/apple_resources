

- WebKit
- WebHistory
-  removeItems(\_:) Deprecated

Instance Method

# removeItems(\_:)

Removes the specified items from the web history.

macOS 10.3–10.14Deprecated

``` source
func removeItems(_ items: [Any]!)
```

## Parameters 

`items`  

An array of web history items to remove.

## Discussion

When successful, this method posts a notification (WebHistoryItemsRemovedNotification).

## See Also

### Adding and Removing History Items

func addItems([Any]!)

Inserts or updates the specified items in the web history.

Deprecated

func removeAllItems()

Removes all items from the web history.

Deprecated

