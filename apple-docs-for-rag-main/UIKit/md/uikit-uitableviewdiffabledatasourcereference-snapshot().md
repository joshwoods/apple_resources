

- UIKit
- UITableViewDiffableDataSourceReference
-  snapshot() 

Instance Method

# snapshot()

Returns a representation of the current state of the data in the table view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func snapshot() -> NSDiffableDataSourceSnapshotReference
```

## See Also

### Updating data

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

var defaultRowAnimation: UITableView.RowAnimation

The default type of animation to use when inserting or deleting rows.

