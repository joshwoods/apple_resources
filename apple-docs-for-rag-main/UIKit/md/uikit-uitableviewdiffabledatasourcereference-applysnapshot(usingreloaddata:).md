

- UIKit
- UITableViewDiffableDataSourceReference
-  applySnapshot(usingReloadData:) 

Instance Method

# applySnapshot(usingReloadData:)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func applySnapshot(usingReloadData snapshot: NSDiffableDataSourceSnapshotReference)
```

## Parameters 

`snapshot`  

The snapshot that reflects the new state of the data in the table view.

## Discussion

The system interrupts any ongoing item animations and immediately reloads the table view’s content.

You can safely call this method from a background queue, but you must do so consistently in your app. Always call this method exclusively from the main queue or from a background queue.

## See Also

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshotReference

Returns a representation of the current state of the data in the table view.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

var defaultRowAnimation: UITableView.RowAnimation

The default type of animation to use when inserting or deleting rows.

