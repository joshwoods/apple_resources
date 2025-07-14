

- UIKit
- UITableViewHeaderFooterView
-  backgroundView 

Instance Property

# backgroundView

The background view of the header or footer.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var backgroundView: UIView? { get set }
```

## Mentioned in 

Adding headers and footers to table sections

## Discussion

The view in this property appears behind the view in the contentView property and displays static background content behind the header or footer. For example, you might assign an image view to this property and use it to display a custom background image.

A background configuration is mutually exclusive with background views, so you must use one approach or the other. Setting a non-`nil` value for this property resets backgroundConfiguration to `nil`.

## See Also

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the view.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the view automatically updates its background configuration when its state changes.

