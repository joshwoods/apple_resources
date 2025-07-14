

- AppKit
- NSComboButton
-  style 

Instance Property

# style

The appearance setting that determines how the button presents its menu .

macOS 13.0+

``` source
@MainActor
var style: NSComboButton.Style { get set }
```

## Discussion

The default value of this property is NSComboButton.Style.split.

## See Also

### Configuring the Button Appearance

enum Style

Constants that indicate how a combo button presents its menu.

var title: String

The localized string that the button displays.

var image: NSImage?

The image that the button displays.

var imageScaling: NSImageScaling

The scaling behavior to apply to the button’s image.

