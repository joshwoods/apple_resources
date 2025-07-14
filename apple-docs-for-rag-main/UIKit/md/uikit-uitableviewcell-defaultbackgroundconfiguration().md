

- UIKit
- UITableViewCell
-  defaultBackgroundConfiguration() 

Instance Method

# defaultBackgroundConfiguration()

Retrieves a background configuration with system default values.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
@MainActor @preconcurrency
func defaultBackgroundConfiguration() -> UIBackgroundConfiguration
```

## Return Value

A default background configuration. The system determines default values for the configuration according to the section where the cell appears.

## See Also

### Configuring the background

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The view to use as the background of the cell.

var selectedBackgroundView: UIView?

The view to use as the background for a selected cell.

var multipleSelectionBackgroundView: UIView?

The background view to use for a selected cell when the table view allows multiple row selections.

