

- UIKit
- UICollectionViewCell
-  backgroundView 

Instance Property

# backgroundView

The view that displays behind the cell’s other content.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var backgroundView: UIView? { get set }
```

## Discussion

Use this property to assign a custom background view to the cell. The background view appears behind the content view and its frame automatically adjusts so that it fills the bounds of the cell.

A background configuration is mutually exclusive with background views, so you must use one approach or the other. Setting a non-`nil` value for this property resets backgroundConfiguration to `nil`.

## See Also

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var selectedBackgroundView: UIView?

The view that displays just above the background view for a selected cell.

