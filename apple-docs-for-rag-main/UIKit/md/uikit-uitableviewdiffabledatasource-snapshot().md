

- UIKit
- UITableViewDiffableDataSource
-  snapshot() 

Instance Method

# snapshot()

Returns a representation of the current state of the data in the table view.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
@MainActor @preconcurrency
func snapshot() -> NSDiffableDataSourceSnapshot
```

## Return Value

A snapshot containing section and item identifiers in the order that they appear in the UI.

## See Also

### Updating data

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool) async

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>) async

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

var defaultRowAnimation: UITableView.RowAnimation

The default type of animation to use when inserting or deleting rows.

