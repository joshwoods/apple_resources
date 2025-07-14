

- UIKit
- UITableViewHeaderFooterView
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

A default background configuration. The system determines default values for the configuration according to the section where the view appears.

## See Also

### Configuring the background

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the view.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the view automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The background view of the header or footer.

