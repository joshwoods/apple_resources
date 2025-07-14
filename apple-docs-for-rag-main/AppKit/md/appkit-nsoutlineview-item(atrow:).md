

- AppKit
- NSOutlineView
-  item(atRow:) 

Instance Method

# item(atRow:)

Returns the item associated with a given row.

macOS

``` source
@MainActor
func item(atRow row: Int) -> Any?
```

## Parameters 

`row`  

The index of a row in the receiver.

## Return Value

The item associated with `row`.

## See Also

### Converting Between Items and Rows

func row(forItem: Any?) -> Int

Returns the row associated with a given item.

