

- AppKit
- NSColorPicker
-  buttonToolTip 

Instance Property

# buttonToolTip

The tool tip that is shown when the mouse cursor is over the color picker’s button image.

macOS

``` source
var buttonToolTip: String { get }
```

## Discussion

Override this property’s getter method to provide a custom tool tip. The default implementation returns the name of the receiver’s class. If you want the color picker to have no tool tip, return an empty string.

## See Also

### Customizing the Color Picker

var minContentSize: NSSize

The minimum content size.

