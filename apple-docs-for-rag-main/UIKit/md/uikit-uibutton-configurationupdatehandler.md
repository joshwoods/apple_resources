

- UIKit
- UIButton
-  configurationUpdateHandler 

Instance Property

# configurationUpdateHandler

A closure that executes when the button state changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler? { get set }
```

## Discussion

Use this property as an alternative to overriding updateConfiguration(). Set a closure to respond to button state changes by updating the button configuration.

In iOS 18 and later, UIKit supports automatic trait tracking inside this closure for traits from this button’s `traitCollection`. For more information, see Automatic trait tracking.

## See Also

### Buttons

func updateConfiguration()

Updates the button configuration in response to a button state change.

