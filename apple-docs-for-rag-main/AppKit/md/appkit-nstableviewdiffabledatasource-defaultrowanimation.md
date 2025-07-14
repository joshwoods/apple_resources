

- AppKit
- NSTableViewDiffableDataSource
-  defaultRowAnimation 

Instance Property

# defaultRowAnimation

The default animation the UI uses to show differences between rows.

macOS 11.0+

``` source
var defaultRowAnimation: NSTableView.AnimationOptions
```

## Discussion

The default value of this property is effectFade.

If you set the value of this property, the new value becomes the default row animation for the next update that uses apply(_:animatingDifferences:completion:).

## See Also

### Updating Data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the table view.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

