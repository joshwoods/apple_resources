

- UIKit
- UITableViewCell
-  selectedBackgroundView 

Instance Property

# selectedBackgroundView

The view to use as the background for a selected cell.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectedBackgroundView: UIView? { get set }
```

## Discussion

UITableViewCell adds the value of this property as a subview only when the cell has a selected state. It adds the selected background view as a subview directly above the background view (backgroundView) if it isn’t `nil`, or behind all other views. Calling setSelected(_:animated:) causes the selected background view to animate in and out with an alpha fade.

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

var multipleSelectionBackgroundView: UIView?

The background view to use for a selected cell when the table view allows multiple row selections.

