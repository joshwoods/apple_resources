

- UIKit
- UIButton
-  updateConfiguration() 

Instance Method

# updateConfiguration()

Updates the button configuration in response to a button state change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func updateConfiguration()
```

## Discussion

Override this method in your subclass to respond changes to the button’s state. Make any necessary changes and update the button’s configuration.

Don’t call this method directly. Call setNeedsUpdateConfiguration() to request an update to your button.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this button’s `traitCollection`. For more information, see Automatic trait tracking.

## See Also

### Buttons

var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler?

A closure that executes when the button state changes.

