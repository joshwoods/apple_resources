

- UIKit
- UIButton
-  UIButton.ConfigurationUpdateHandler 

Type Alias

# UIButton.ConfigurationUpdateHandler

A closure to update the configuration of a button.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
typealias ConfigurationUpdateHandler = (UIButton) -> Void
```

## Parameters 

`button`  

The button to update.

## See Also

### Managing the appearance with a configuration object

var configuration: UIButton.Configuration?

The configuration for the button’s appearance.

var automaticallyUpdatesConfiguration: Bool

A Boolean value that determines whether the button configuration changes when button’s state changes.

func setNeedsUpdateConfiguration()

Requests the system update the button configuration.

func updateConfiguration()

Updates the button configuration in response to a button state change.

var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler?

A closure that executes when the button state changes.

