

- AppKit
- NSOutlineView
-  row(forItem:) 

Instance Method

# row(forItem:)

Returns the row associated with a given item.

macOS

``` source
@MainActor
func row(forItem item: Any?) -> Int
```

## Parameters 

`item`  

An item in the receiver.

## Return Value

The row associated with `item`, or `–1` if `item` is `nil` or cannot be found.

## See Also

### Converting Between Items and Rows

func item(atRow: Int) -> Any?

Returns the item associated with a given row.

