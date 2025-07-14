

- UIKit
- UITableViewHeaderFooterView
-  backgroundConfiguration 

Instance Property

# backgroundConfiguration

The current background configuration of the view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
var backgroundConfiguration: UIBackgroundConfiguration? { get set }
```

## Discussion

Using a background configuration, you can obtain system default background styling for a variety of different view states. Create a background configuration with one of the default system styles, customize the configuration to match your view’s style as necessary, and assign the configuration to this property.

```
var backgroundConfig = UIBackgroundConfiguration.listPlainHeaderFooter()
backgroundConfig.backgroundColor = .systemGray
header.backgroundConfiguration = backgroundConfig
```

A background configuration is mutually exclusive with background views, so you must use one approach or the other. Setting a non-`nil` value for this property resets the following APIs to `nil`:

- backgroundColor

- backgroundView

## See Also

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the view automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The background view of the header or footer.

