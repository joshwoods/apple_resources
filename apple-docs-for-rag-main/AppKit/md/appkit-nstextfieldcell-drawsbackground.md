

- AppKit
- NSTextFieldCell
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean value that indicates whether the cell draws its background color.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

When the value of this property is true, the cell draws its background color. In order to prevent inconsistent rendering, background color rendering is automatically disabled for rounded-bezel text fields.

## See Also

### Related Documentation

var drawsBackground: Bool

A Boolean value that controls whether the text field’s cell draws a background color behind the text.

### Controlling the Background

var backgroundColor: NSColor?

The color of the cell’s background.

