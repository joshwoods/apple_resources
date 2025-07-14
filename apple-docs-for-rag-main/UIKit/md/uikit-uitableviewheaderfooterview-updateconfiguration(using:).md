

- UIKit
- UITableViewHeaderFooterView
-  updateConfiguration(using:) 

Instance Method

# updateConfiguration(using:)

Updates the view’s configuration using the current state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @objc(_bridgedUpdateConfigurationUsingState:) @preconcurrency
dynamic func updateConfiguration(using state: UIViewConfigurationState)
```

## Discussion

Avoid calling this method directly. Instead, use setNeedsUpdateConfiguration() to request an update.

Override this method in a subclass to update the view’s configuration using the provided state.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this view’s `traitCollection`. For more information, see Automatic trait tracking.

## See Also

### Table view headers and footers

var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler?

A block for handling updates to the view’s configuration using the current state.

