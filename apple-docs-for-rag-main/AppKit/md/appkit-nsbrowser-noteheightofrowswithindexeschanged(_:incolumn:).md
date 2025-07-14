

- AppKit
- NSBrowser
-  noteHeightOfRowsWithIndexesChanged(\_:inColumn:) 

Instance Method

# noteHeightOfRowsWithIndexesChanged(\_:inColumn:)

Immediately retiles the browser’s columns using row heights specified by the browser’s delegate.

macOS 10.6+

``` source
@MainActor
func noteHeightOfRowsWithIndexesChanged(
    _ indexSet: IndexSet,
    inColumn columnIndex: Int
)
```

## Parameters 

`indexSet`  

The indexes of the rows to resize.

`columnIndex`  

The column to retile.

## Discussion

The browser’s delegate must implement

## See Also

### Updating Browsers

func reloadData(forRowIndexes: IndexSet, inColumn: Int)

Updates the rows in the column with the specified column index with indexes in the specified set.

