

- AppKit
- NSTableHeaderView
-  column(at:) 

Instance Method

# column(at:)

Returns the index of the column whose header lies under `aPoint` in the receiver, or –1 if no such column is found.

macOS

``` source
@MainActor
func column(at point: NSPoint) -> Int
```

## Discussion

`aPoint` is expressed in the receiver’s coordinate system.

## See Also

### Utility methods

func headerRect(ofColumn: Int) -> NSRect

Returns the rectangle containing the header tile for the column at `columnIndex`.

