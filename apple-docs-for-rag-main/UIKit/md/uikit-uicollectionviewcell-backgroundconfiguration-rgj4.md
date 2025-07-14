

- UIKit
- UICollectionViewCell
-  backgroundConfiguration 

Instance Property

# backgroundConfiguration

The current background configuration of the cell.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
var backgroundConfiguration: UIBackgroundConfiguration? { get set }
```

## Discussion

Using a background configuration, you can obtain system default background styling for a variety of different cell states. Create a background configuration with one of the default system styles, customize the configuration to match your cell’s style as necessary, and assign the configuration to this property.

```
var backgroundConfig = UIBackgroundConfiguration.listPlainCell()

// Set a nil background color to use the view's tint color. 
backgroundConfig.backgroundColor = nil 

cell.backgroundConfiguration = backgroundConfig 
```

A background configuration is mutually exclusive with background views, so you must use one approach or the other. Setting a non-`nil` value for this property resets the following APIs to `nil`:

- backgroundColor

- backgroundView

- selectedBackgroundView

## See Also

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The view that displays behind the cell’s other content.

var selectedBackgroundView: UIView?

The view that displays just above the background view for a selected cell.

