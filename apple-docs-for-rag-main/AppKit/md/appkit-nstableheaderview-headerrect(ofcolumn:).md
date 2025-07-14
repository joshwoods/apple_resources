

- AppKit
- NSTableHeaderView
-  headerRect(ofColumn:) 

Instance Method

# headerRect(ofColumn:)

Returns the rectangle containing the header tile for the column at `columnIndex`.

macOS

``` source
@MainActor
func headerRect(ofColumn column: Int) -> NSRect
```

## Discussion

Raises an `NSInternalInconsistencyException` if `columnIndex` is out of bounds.

## See Also

### Related Documentation

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the column at the specified index.

### Utility methods

func column(at: NSPoint) -> Int

Returns the index of the column whose header lies under `aPoint` in the receiver, or –1 if no such column is found.

