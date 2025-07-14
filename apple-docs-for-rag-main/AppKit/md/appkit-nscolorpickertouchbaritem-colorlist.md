

- AppKit
- NSColorPickerTouchBarItem
-  colorList 

Instance Property

# colorList

The list of colors displayed in the color picker.

macOS 10.12.2+

``` source
@MainActor
var colorList: NSColorList! { get set }
```

## Discussion

Defaults to the standard system color list.

Note that setting a custom color list disables the additional tints and shades that appear when the user sustains a touch.

## See Also

### Configuring the color picker

var allowedColorSpaces: [NSColorSpace]?

Controls the color spaces that the color picker can produce.

var showsAlpha: Bool

A Boolean value that controls whether the color picker allows picking of colors with alpha values other than `1.0`.

var isEnabled: Bool

A Boolean value that determines whether the color picker is enabled.

