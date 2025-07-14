

- UIKit
- UITableViewDiffableDataSourceReference
-  indexPath(forItemIdentifier:) 

Instance Method

# indexPath(forItemIdentifier:)

Returns an index path for the item with the specified identifier in the table view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func indexPath(forItemIdentifier identifier: Any) -> IndexPath?
```

## Parameters 

`identifier`  

The identifier of the item in the table view.

## Return Value

The item’s index path, or `nil` if no item is found with the provided item identifier.

## Discussion

This method is a constant time operation, O(1), which means you can look up an index path from its corresponding item identifier with no significant overhead.

## See Also

### Identifying items

func itemIdentifier(for: IndexPath) -> Any?

Returns an identifier for the item at the specified index path in the table view.

