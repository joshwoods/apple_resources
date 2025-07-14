

- AppKit
- NSColorWell
-  colorWellStyle 

Instance Property

# colorWellStyle

The appearance and interaction style to apply to the color well.

macOS 13.0+

``` source
@MainActor
var colorWellStyle: NSColorWell.Style { get set }
```

## Discussion

The value of this property determines how the color well presents itself, and how interactions affect it. For details, see NSColorWell.Style.

## See Also

### Configuring the Appearance

enum Style

Constants that specify the appearance and interaction modes for a color well.

var image: NSImage?

The image to display on the button portion of a color well that adopts the expanded style.

var isBordered: Bool

A Boolean value that determines whether the color well has a border.

Deprecated

