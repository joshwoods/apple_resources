

- UIKit
- UIButton
-  configuration 

Instance Property

# configuration

The configuration for the button’s appearance.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
var configuration: UIButton.Configuration? { get set }
```

## Discussion

Setting a configuration opts the button into a configuration system based on UIButton.Configuration. This configuration supports several options and behaviors unavailable with other configuration methods. Features include subtitle labels, extended control over background appearance, ways to transform the button configuration when the button changes state, and integration with macOS when building with Mac Catalyst.

When using a configuration, the button ignores deprecated methods and properties of UIButton. You can combine most other methods and properties of UIButton with a configuration. If you have existing code to configure a button, you can set this property to take advantage of additional configuration features.

If the configuration is `nil`, other supported properties and methods of UIButton, such as setTitle(_:for:) , control the appearance of the button.

## See Also

### Managing the appearance with a configuration object

var automaticallyUpdatesConfiguration: Bool

A Boolean value that determines whether the button configuration changes when button’s state changes.

func setNeedsUpdateConfiguration()

Requests the system update the button configuration.

func updateConfiguration()

Updates the button configuration in response to a button state change.

var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler?

A closure that executes when the button state changes.

typealias ConfigurationUpdateHandler

A closure to update the configuration of a button.

