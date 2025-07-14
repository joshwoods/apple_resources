

- AppKit
- NSColorWell
-  NSColorWell.Style 

Enumeration

# NSColorWell.Style

Constants that specify the appearance and interaction modes for a color well.

macOS 13.0+

``` source
enum Style
```

## Topics

### Getting the Style Option

case `default`

The default style for color wells.

case minimal

A style that adds minimal adornments to the color well.

case expanded

A style that supports a color picker popover for fast interactions, and adds a dedicated button to display the color panel.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the Appearance

var colorWellStyle: NSColorWell.Style

The appearance and interaction style to apply to the color well.

var image: NSImage?

The image to display on the button portion of a color well that adopts the expanded style.

var isBordered: Bool

A Boolean value that determines whether the color well has a border.

Deprecated

