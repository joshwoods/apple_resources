

- AppKit
- NSTextField
-  isBezeled 

Instance Property

# isBezeled

A Boolean value that controls whether the text field draws a bezeled background around its contents.

macOS

``` source
@MainActor
var isBezeled: Bool { get set }
```

## Discussion

If true, the text field draws a bezel and sets drawsBackground to false; if false, it doesn’t draw a bezeled background.

## See Also

### Controlling the Background

var backgroundColor: NSColor?

The color of the background the text field’s cell draws behind the text.

var drawsBackground: Bool

A Boolean value that controls whether the text field’s cell draws a background color behind the text.

var bezelStyle: NSTextField.BezelStyle

The text field’s bezel style, square or rounded.

enum BezelStyle

The style of bezel the text field displays.

