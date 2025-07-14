

- UIKit
- UITableViewHeaderFooterView
-  configurationUpdateHandler 

Instance Property

# configurationUpdateHandler

A block for handling updates to the view’s configuration using the current state.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler? { get set }
```

## Discussion

A configuration update handler provides an alternative approach to overriding updateConfiguration(using:) in a subclass. Set a configuration update handler to update the header footer view’s configuration using the new state in response to a configuration state change.

Setting the value of this property calls setNeedsUpdateConfiguration(). The system calls this handler after calling updateConfiguration(using:).

In iOS 18 and later, UIKit supports automatic trait tracking inside this closure for traits from this view’s `traitCollection`. For more information, see Automatic trait tracking.

## See Also

### Table view headers and footers

func updateConfiguration(using: UIViewConfigurationState)

Updates the view’s configuration using the current state.

