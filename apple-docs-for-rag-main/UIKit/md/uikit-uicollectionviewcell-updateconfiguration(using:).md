

- UIKit
- UICollectionViewCell
-  updateConfiguration(using:) 

Instance Method

# updateConfiguration(using:)

Updates the cell’s configuration using the current state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @objc(_bridgedUpdateConfigurationUsingState:) @preconcurrency
dynamic func updateConfiguration(using state: UICellConfigurationState)
```

## Discussion

Avoid calling this method directly. Instead, use setNeedsUpdateConfiguration() to request an update.

Override this method in a subclass to update the cell’s configuration using the provided state.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this cell’s `traitCollection`. For more information, see Automatic trait tracking.

## See Also

### Collection view cells

var configurationUpdateHandler: UICollectionViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

