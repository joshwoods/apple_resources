

- AppKit
- NSColorPickerTouchBarItem
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that determines whether the color picker is enabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

If the picker is currently displayed as a popover, and you set the value of this property to false, the picker is dismissed.

## See Also

### Configuring the color picker

var colorList: NSColorList!

The list of colors displayed in the color picker.

var allowedColorSpaces: [NSColorSpace]?

Controls the color spaces that the color picker can produce.

var showsAlpha: Bool

A Boolean value that controls whether the color picker allows picking of colors with alpha values other than `1.0`.

