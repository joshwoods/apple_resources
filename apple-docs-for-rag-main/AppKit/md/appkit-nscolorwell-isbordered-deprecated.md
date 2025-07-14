

- AppKit
- NSColorWell
-  isBordered Deprecated

Instance Property

# isBordered

A Boolean value that determines whether the color well has a border.

macOS 10.0–15.4Deprecated

``` source
@MainActor
var isBordered: Bool { get set }
```

Deprecated

This property will be deprecated in a future release.

## Discussion

If the value of this property is true, the color well has a border; if it’s false, the color well doesn’t have a border. The default value of this property is true.

A borderless color well doesn’t display the Colors window when someone clicks it.

## See Also

### Configuring the Appearance

var colorWellStyle: NSColorWell.Style

The appearance and interaction style to apply to the color well.

enum Style

Constants that specify the appearance and interaction modes for a color well.

var image: NSImage?

The image to display on the button portion of a color well that adopts the expanded style.

