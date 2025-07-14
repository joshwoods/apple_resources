

- AppKit
- NSComboButton
-  image 

Instance Property

# image

The image that the button displays.

macOS 13.0+

``` source
@MainActor
var image: NSImage? { get set }
```

## Discussion

The combo button scales the image to fit within its bounds. Use the imageScaling property to specify the scaling behavior to use with your image.

## See Also

### Configuring the Button Appearance

var style: NSComboButton.Style

The appearance setting that determines how the button presents its menu .

enum Style

Constants that indicate how a combo button presents its menu.

var title: String

The localized string that the button displays.

var imageScaling: NSImageScaling

The scaling behavior to apply to the button’s image.

