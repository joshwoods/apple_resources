

- UIKit
- UITableViewHeaderFooterView
-  configurationState 

Instance Property

# configurationState

The current configuration state of the view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @objc(_bridgedConfigurationState) @preconcurrency
dynamic var configurationState: UIViewConfigurationState { get }
```

## Discussion

To add your own custom state, see UIConfigurationStateCustomKey.

## See Also

### Managing the state

func setNeedsUpdateConfiguration()

Informs the view to update its configuration for its current state.

func updateConfiguration(using: UIViewConfigurationState)

Updates the view’s configuration using the current state.

var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler?

A block for handling updates to the view’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the view’s configuration using the current state.

