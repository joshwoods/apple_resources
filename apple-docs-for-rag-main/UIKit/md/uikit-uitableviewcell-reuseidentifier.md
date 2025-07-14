

- UIKit
- UITableViewCell
-  reuseIdentifier 

Instance Property

# reuseIdentifier

A string for identifying a reusable cell.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var reuseIdentifier: String? { get }
```

## Discussion

The reuse identifier is associated with a UITableViewCell object that the table-view’s delegate creates with the intent to reuse it as the basis (for performance reasons) for multiple rows of a table view. It is assigned to the cell object in initWithFrame:reuseIdentifier: and cannot be changed thereafter. A UITableView object maintains a queue (or list) of the currently reusable cells, each with its own reuse identifier, and makes them available to the delegate in the dequeueReusableCell(withIdentifier:) method.

## See Also

### Reusing cells

func prepareForReuse()

Prepares a reusable cell for reuse by the table view’s delegate.

