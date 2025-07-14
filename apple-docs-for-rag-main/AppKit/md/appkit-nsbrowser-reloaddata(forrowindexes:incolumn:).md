

- AppKit
- NSBrowser
-  reloadData(forRowIndexes:inColumn:) 

Instance Method

# reloadData(forRowIndexes:inColumn:)

Updates the rows in the column with the specified column index with indexes in the specified set.

macOS 10.6+

``` source
@MainActor
func reloadData(
    forRowIndexes rowIndexes: IndexSet,
    inColumn column: Int
)
```

## Parameters 

`rowIndexes`  

The set of row indexes of the rows to be updated.

`column`  

The column containing the rows to be updated.

## See Also

### Updating Browsers

func noteHeightOfRowsWithIndexesChanged(IndexSet, inColumn: Int)

Immediately retiles the browser’s columns using row heights specified by the browser’s delegate.

