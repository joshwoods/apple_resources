

- AppKit
- NSTableViewDiffableDataSource
-  snapshot() 

Instance Method

# snapshot()

Returns a representation of the current state of the data in the table view.

macOS 11.0+

``` source
func snapshot() -> NSDiffableDataSourceSnapshot
```

## Return Value

A snapshot that contains row and item identifiers in the order they appear in the UI.

## See Also

### Updating Data

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

var defaultRowAnimation: NSTableView.AnimationOptions

The default animation the UI uses to show differences between rows.

