

- UIKit
- UITableViewCell
-  backgroundView 

Instance Property

# backgroundView

The view to use as the background of the cell.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var backgroundView: UIView? { get set }
```

## Discussion

UITableViewCell adds the background view as a subview behind all other views and uses its current frame location.

A background configuration is mutually exclusive with background views, so you must use one approach or the other. Setting a non-`nil` value for this property resets backgroundConfiguration to `nil`.

## See Also

### Related Documentation

var contentView: UIView

The content view of the cell object.

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var selectedBackgroundView: UIView?

The view to use as the background for a selected cell.

var multipleSelectionBackgroundView: UIView?

The background view to use for a selected cell when the table view allows multiple row selections.

