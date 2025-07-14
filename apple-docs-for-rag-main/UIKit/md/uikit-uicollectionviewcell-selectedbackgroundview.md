

- UIKit
- UICollectionViewCell
-  selectedBackgroundView 

Instance Property

# selectedBackgroundView

The view that displays just above the background view for a selected cell.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectedBackgroundView: UIView? { get set }
```

## Discussion

You can use this view to give a selected cell a custom appearance. When the cell has a selected state, this view layers above the backgroundView and behind the contentView.

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

The view that displays behind the cell’s other content.

