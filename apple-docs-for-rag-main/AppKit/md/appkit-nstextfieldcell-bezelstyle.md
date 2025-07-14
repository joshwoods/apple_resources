

- AppKit
- NSTextFieldCell
-  bezelStyle 

Instance Property

# bezelStyle

The bezel style to use when drawing the text field.

macOS

``` source
@MainActor
var bezelStyle: NSTextField.BezelStyle { get set }
```

## Discussion

To set the bezel style, you must have already set the the text field’s isBezeled method with an argument of true. For a list of bezel styles, see NSTextField.BezelStyle.

## See Also

### Setting the Bezel Style

enum BezelStyle

The style of bezel the text field displays.

