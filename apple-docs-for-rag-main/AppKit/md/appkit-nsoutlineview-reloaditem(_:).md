

- AppKit
- NSOutlineView
-  reloadItem(\_:) 

Instance Method

# reloadItem(\_:)

Reloads and redisplays the data for the given item.

macOS

``` source
@MainActor
func reloadItem(_ item: Any?)
```

## Parameters 

`item`  

The item to reload and display.

## Discussion

Reloading the cell views associated with `item` occurs only in apps that link against macOS 10.12 and later.

This method may cause the outline view to change its selection without calling the outlineViewSelectionDidChange(_:) delegate method.

## See Also

### Redisplaying Information

func reloadItem(Any?, reloadChildren: Bool)

Reloads a given item and, optionally, its children.

