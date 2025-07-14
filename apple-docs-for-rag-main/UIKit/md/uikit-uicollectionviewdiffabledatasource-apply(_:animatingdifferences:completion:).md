

- UIKit
- UICollectionViewDiffableDataSource
-  apply(\_:animatingDifferences:completion:) 

Instance Method

# apply(\_:animatingDifferences:completion:)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
@MainActor @preconcurrency
func apply(
    _ snapshot: NSDiffableDataSourceSnapshot,
    animatingDifferences: Bool = true,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`snapshot`  

The snapshot that reflects the new state of the data in the collection view.

`animatingDifferences`  

If true, the system animates the updates to the collection view. If false, the system doesn’t animate the updates to the collection view.

`completion`  

A closure to execute when the animations are complete. This closure has no return value and takes no parameters. The system calls this closure from the main queue.

## Discussion

The diffable data source computes the difference between the collection view’s current state and the new state in the applied snapshot, which is an O(*n*) operation, where *n* is the number of items in the snapshot.

You can safely call this method from a background queue, but you must do so consistently in your app. Always call this method exclusively from the main queue or from a background queue.

## See Also

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the collection view.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool) async

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>) async

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

