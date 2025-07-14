

- AppKit
- NSCollectionViewDiffableDataSource
-  itemIdentifier(for:) 

Instance Method

# itemIdentifier(for:)

Returns an identifier for the item at the specified index path in the collection view.

macOS 10.15.1+

``` source
func itemIdentifier(for indexPath: IndexPath) -> ItemIdentifierType?
```

## Parameters 

`indexPath`  

The index path of the item in the collection view.

## Return Value

The item’s identifier, or `nil` if no item is found at the provided index path.

## Discussion

This method is a constant time operation, O(1), which means you can look up an item identifier from its corresponding index path with no significant overhead.

## See Also

### Identifying Items

func indexPath(for: ItemIdentifierType) -> IndexPath?

Returns an index path for the item with the specified identifier in the collection view.

