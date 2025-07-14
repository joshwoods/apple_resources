

- UIKit
- UICollectionViewDiffableDataSource
-  apply(\_:animatingDifferences:) 

Instance Method

# apply(\_:animatingDifferences:)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
func apply(
    _ snapshot: NSDiffableDataSourceSnapshot,
    animatingDifferences: Bool = true
) async
```

## See Also

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the collection view.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>) async

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

