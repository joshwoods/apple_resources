

- UIKit
- UITableViewDiffableDataSourceReference
-  defaultRowAnimation 

Instance Property

# defaultRowAnimation

The default type of animation to use when inserting or deleting rows.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var defaultRowAnimation: UITableView.RowAnimation { get set }
```

## Discussion

The default value of this property is UITableView.RowAnimation.automatic.

If you set the value of this property, the new value becomes the default row animation for the next update that uses applySnapshot(_:animatingDifferences:) or applySnapshot(_:animatingDifferences:completion:).

## See Also

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshotReference

Returns a representation of the current state of the data in the table view.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshot(usingReloadData: NSDiffableDataSourceSnapshotReference, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

