

- UIKit
- UICollectionViewDiffableDataSource
-  indexPath(for:) 

Instance Method

# indexPath(for:)

Returns an index path for the item with the specified identifier in the collection view.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
@MainActor @preconcurrency
func indexPath(for itemIdentifier: ItemIdentifierType) -> IndexPath?
```

## Parameters 

`itemIdentifier`  

The identifier of the item in the collection view.

## Return Value

The item’s index path, or `nil` if no item is found with the provided item identifier.

## Discussion

This method is a constant time operation, O(1), which means you can look up an index path from its corresponding item identifier with no significant overhead.

## See Also

### Identifying items

func itemIdentifier(for: IndexPath) -> ItemIdentifierType?

Returns an identifier for the item at the specified index path in the collection view.

