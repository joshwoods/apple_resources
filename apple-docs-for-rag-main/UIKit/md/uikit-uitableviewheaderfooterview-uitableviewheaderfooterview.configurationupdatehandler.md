

- UIKit
- UITableViewHeaderFooterView
-  UITableViewHeaderFooterView.ConfigurationUpdateHandler 

Type Alias

# UITableViewHeaderFooterView.ConfigurationUpdateHandler

The type of block for handling updates to the view’s configuration using the current state.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
typealias ConfigurationUpdateHandler = (UITableViewHeaderFooterView, UIViewConfigurationState) -> Void
```

## Parameters 

`headerFooterView`  

The header footer view to configure.

`state`  

The new state to use for updating the header footer view’s configuration.

## See Also

### Managing the state

var configurationState: UIViewConfigurationState

The current configuration state of the view.

func setNeedsUpdateConfiguration()

Informs the view to update its configuration for its current state.

func updateConfiguration(using: UIViewConfigurationState)

Updates the view’s configuration using the current state.

var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler?

A block for handling updates to the view’s configuration using the current state.

