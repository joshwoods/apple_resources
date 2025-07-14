

- AppKit
- NSComboButton
-  imageScaling 

Instance Property

# imageScaling

The scaling behavior to apply to the button’s image.

macOS 13.0+

``` source
@MainActor
var imageScaling: NSImageScaling { get set }
```

## Discussion

The default value of this property is NSImageScaling.scaleProportionallyDown.

## See Also

### Configuring the Button Appearance

var style: NSComboButton.Style

The appearance setting that determines how the button presents its menu .

enum Style

Constants that indicate how a combo button presents its menu.

var title: String

The localized string that the button displays.

var image: NSImage?

The image that the button displays.

