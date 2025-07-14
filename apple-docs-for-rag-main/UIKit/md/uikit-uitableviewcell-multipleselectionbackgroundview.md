

- UIKit
- UITableViewCell
-  multipleSelectionBackgroundView 

Instance Property

# multipleSelectionBackgroundView

The background view to use for a selected cell when the table view allows multiple row selections.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var multipleSelectionBackgroundView: UIView? { get set }
```

## Discussion

If this property isn’t `nil`, this view becomes the background view for a selected cell when the table view allows multiple row selections. You enable multiple row selections through the allowsMultipleSelection and allowsMultipleSelectionDuringEditing properties of UITableView.

A background configuration is mutually exclusive with background views, so you must use one approach or the other. Setting a non-`nil` value for this property resets backgroundConfiguration to `nil`.

## See Also

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The view to use as the background of the cell.

var selectedBackgroundView: UIView?

The view to use as the background for a selected cell.

