

- UIKit
- UITableViewDiffableDataSourceReference
-  applySnapshot(\_:animatingDifferences:) 

Instance Method

# applySnapshot(\_:animatingDifferences:)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func applySnapshot(
    _ snapshot: NSDiffableDataSourceSnapshotReference,
    animatingDifferences: Bool
)
```

## Parameters 

`snapshot`  

The snapshot that reflects the new state of the data in the table view.

`animatingDifferences`  

If true, the system animates the updates to the table view. If false, the system doesn’t animate the updates to the table view.

## Discussion

The diffable data source computes the difference between the table view’s current state and the new state in the applied snapshot, which is an O(*n*) operation, where *n* is the number of items in the snapshot.

You can safely call this method from a background queue, but you must do so consistently in your app. Always call this method exclusively from the main queue or from a background queue.

## See Also

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshotReference

Returns a representation of the current state of the data in the table view.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

var defaultRowAnimation: UITableView.RowAnimation

The default type of animation to use when inserting or deleting rows.

