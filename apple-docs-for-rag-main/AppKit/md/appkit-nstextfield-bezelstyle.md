

- AppKit
- NSTextField
-  bezelStyle 

Instance Property

# bezelStyle

The text field’s bezel style, square or rounded.

macOS

``` source
@MainActor
var bezelStyle: NSTextField.BezelStyle { get set }
```

## Discussion

To enable a bezel for a text field, set isBezeled to true, then set the bezel style. See NSTextField.BezelStyle for available bezel styles.

Note

When you set this property to NSTextField.BezelStyle.roundedBezel, the text field doesn’t wrap the text. It displays using a single line.

## See Also

### Controlling the Background

var backgroundColor: NSColor?

The color of the background the text field’s cell draws behind the text.

var drawsBackground: Bool

A Boolean value that controls whether the text field’s cell draws a background color behind the text.

var isBezeled: Bool

A Boolean value that controls whether the text field draws a bezeled background around its contents.

enum BezelStyle

The style of bezel the text field displays.

