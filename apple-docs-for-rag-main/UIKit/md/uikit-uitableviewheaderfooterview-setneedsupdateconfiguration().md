

- UIKit
- UITableViewHeaderFooterView
-  setNeedsUpdateConfiguration() 

Instance Method

# setNeedsUpdateConfiguration()

Informs the view to update its configuration for its current state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateConfiguration()
```

## Discussion

You call this method when you need the view to update its configuration according to the current configuration state. The system calls this method automatically when the view’s configurationState changes, as well as in other circumstances that may require an update. The system might combine multiple requests into a single update.

If you add custom states to the view’s configuration state, make sure to call this method every time those custom states change.

## See Also

### Managing the state

var configurationState: UIViewConfigurationState

The current configuration state of the view.

func updateConfiguration(using: UIViewConfigurationState)

Updates the view’s configuration using the current state.

var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler?

A block for handling updates to the view’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the view’s configuration using the current state.

