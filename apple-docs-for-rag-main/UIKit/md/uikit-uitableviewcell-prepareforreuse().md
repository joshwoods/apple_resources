

- UIKit
- UITableViewCell
-  prepareForReuse() 

Instance Method

# prepareForReuse()

Prepares a reusable cell for reuse by the table view’s delegate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func prepareForReuse()
```

## Mentioned in 

Configuring the cells for your table

## Discussion

If a UITableViewCell object has a reuse identifier, the table view invokes this method just before returning the object from the `UITableView` method dequeueReusableCell(withIdentifier:). To avoid potential performance issues, you should only reset attributes of the cell that are not related to content, for example, alpha, editing, and selection state. The table view’s delegate in tableView(_:cellForRowAt:) should *always* reset all content when reusing a cell.

The table view doesn’t call this method if the cell object doesn’t have an associated reuse identifier, or if you use reconfigureRows(at:) to update the contents of an existing cell.

If you override this method, you must be sure to invoke the superclass implementation.

## See Also

### Reusing cells

var reuseIdentifier: String?

A string for identifying a reusable cell.

