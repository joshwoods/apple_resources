

- AppKit
- NSCollectionViewDiffableDataSource
-  snapshot() 

Instance Method

# snapshot()

Returns a representation of the current state of the data in the collection view.

macOS 10.15.1+

``` source
func snapshot() -> NSDiffableDataSourceSnapshot
```

## Return Value

A snapshot containing section and item identifiers in the order that they appear in the UI.

## See Also

### Updating Data

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

