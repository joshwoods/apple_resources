

- UIKit
- UIButton
-  setNeedsUpdateConfiguration() 

Instance Method

# setNeedsUpdateConfiguration()

Requests the system update the button configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateConfiguration()
```

## Discussion

Call this method to make the system call updateConfiguration(). The system calls this method automatically when the button’s state changes. If you call this method multiple times before the system calls updateConfiguration(), the system calls updateConfiguration() once.

## See Also

### Managing the appearance with a configuration object

var configuration: UIButton.Configuration?

The configuration for the button’s appearance.

var automaticallyUpdatesConfiguration: Bool

A Boolean value that determines whether the button configuration changes when button’s state changes.

func updateConfiguration()

Updates the button configuration in response to a button state change.

var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler?

A closure that executes when the button state changes.

typealias ConfigurationUpdateHandler

A closure to update the configuration of a button.

