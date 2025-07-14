

- WatchKit
- WKInterfaceTable
-  removeRows(at:) 

Instance Method

# removeRows(at:)

Removes the specified rows from the table.

watchOS 2.0+

``` source
func removeRows(at rows: IndexSet)
```

## Parameters 

`rows`  

An index set corresponding to the rows you want to remove. If any of the indexes are invalid, this method raises an exception.

## Discussion

This method removes row controllers from the table using the same semantics defined by the removeObjects(at:) method of NSMutableArray.

## See Also

### Inserting and Removing Rows

func insertRows(at: IndexSet, withRowType: String)

Inserts rows into the table at the specified indexes.

