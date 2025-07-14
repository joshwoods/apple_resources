

- AppKit
- NSTextField
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean value that controls whether the text field’s cell draws a background color behind the text.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

If true, the text field’s cell draws a background; if false, it draws nothing behind the text.

To prevent inconsistent rendering, `NSTextField` disables background color rendering for text fields with rounded bezels.

## See Also

### Controlling the Background

var backgroundColor: NSColor?

The color of the background the text field’s cell draws behind the text.

var isBezeled: Bool

A Boolean value that controls whether the text field draws a bezeled background around its contents.

var bezelStyle: NSTextField.BezelStyle

The text field’s bezel style, square or rounded.

enum BezelStyle

The style of bezel the text field displays.

