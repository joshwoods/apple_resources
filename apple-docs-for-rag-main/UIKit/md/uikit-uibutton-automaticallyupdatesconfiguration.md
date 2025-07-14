

- UIKit
- UIButton
-  automaticallyUpdatesConfiguration 

Instance Property

# automaticallyUpdatesConfiguration

A Boolean value that determines whether the button configuration changes when button’s state changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var automaticallyUpdatesConfiguration: Bool { get set }
```

## Discussion

Set this property to true to have the button call updated(for:) (Swift) or updatedConfigurationForButton: (Objective-C) when the button state changes and apply the changes to the button. The default value is true.

## See Also

### Managing the appearance with a configuration object

var configuration: UIButton.Configuration?

The configuration for the button’s appearance.

func setNeedsUpdateConfiguration()

Requests the system update the button configuration.

func updateConfiguration()

Updates the button configuration in response to a button state change.

var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler?

A closure that executes when the button state changes.

typealias ConfigurationUpdateHandler

A closure to update the configuration of a button.

