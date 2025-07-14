

- UIKit
- UITableViewCell
-  automaticallyUpdatesBackgroundConfiguration 

Instance Property

# automaticallyUpdatesBackgroundConfiguration

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var automaticallyUpdatesBackgroundConfiguration: Bool { get set }
```

## Discussion

When this value is true, the cell automatically calls `updated(for:)` on its backgroundConfiguration when the cell’s configurationState changes, and applies the updated configuration back to the cell. The default value is true.

If you override updateConfiguration(using:) to manually update and customize the background configuration, disable automatic updates by setting this property to false.

## See Also

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var backgroundView: UIView?

The view to use as the background of the cell.

var selectedBackgroundView: UIView?

The view to use as the background for a selected cell.

var multipleSelectionBackgroundView: UIView?

The background view to use for a selected cell when the table view allows multiple row selections.

