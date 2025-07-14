

- AppKit
- NSComboButton
-  title 

Instance Property

# title

The localized string that the button displays.

macOS 13.0+

``` source
@MainActor
var title: String { get set }
```

## Discussion

The method you use to create the combo button sets the initial value of this property.

## See Also

### Configuring the Button Appearance

var style: NSComboButton.Style

The appearance setting that determines how the button presents its menu .

enum Style

Constants that indicate how a combo button presents its menu.

var image: NSImage?

The image that the button displays.

var imageScaling: NSImageScaling

The scaling behavior to apply to the button’s image.

