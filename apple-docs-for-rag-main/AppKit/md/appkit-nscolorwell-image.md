

- AppKit
- NSColorWell
-  image 

Instance Property

# image

The image to display on the button portion of a color well that adopts the expanded style.

macOS 13.0+

``` source
@MainActor
var image: NSImage? { get set }
```

## Discussion

The color well applies the image only when the colorWellStyle property is set to NSColorWell.Style.expanded.

## See Also

### Configuring the Appearance

var colorWellStyle: NSColorWell.Style

The appearance and interaction style to apply to the color well.

enum Style

Constants that specify the appearance and interaction modes for a color well.

var isBordered: Bool

A Boolean value that determines whether the color well has a border.

Deprecated

