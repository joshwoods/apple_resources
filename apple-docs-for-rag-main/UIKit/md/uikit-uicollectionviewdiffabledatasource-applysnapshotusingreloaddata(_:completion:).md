

- UIKit
- UICollectionViewDiffableDataSource
-  applySnapshotUsingReloadData(\_:completion:) 

Instance Method

# applySnapshotUsingReloadData(\_:completion:)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
func applySnapshotUsingReloadData(
    _ snapshot: NSDiffableDataSourceSnapshot,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`snapshot`  

The snapshot that reflects the new state of the data in the collection view.

`completion`  

A closure to execute when the reload completes. This closure has no return value and takes no parameters. The system calls this closure from the main queue.

## Discussion

The system interrupts any ongoing item animations and immediately reloads the collection view’s content.

You can safely call this method from a background queue, but you must do so consistently in your app. Always call this method exclusively from the main queue or from a background queue.

## See Also

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the collection view.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool) async

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>) async

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

