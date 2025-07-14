

- AppKit
- NSColor
-  textBackgroundColor 

Type Property

# textBackgroundColor

The color to use for the background area behind text.

macOS

``` source
class var textBackgroundColor: NSColor { get }
```

## Discussion

When text is selected, its background color changes to the return value of selectedTextBackgroundColor.

When applied to an NSBox object, this color supports Desktop Tinting in Dark Mode. With Desktop Tinting, the system modifies this color dynamically by incorporating some of the color from the underlying desktop image. The system does not apply this dynamic tinting effect to other types of views.

## See Also

### Text Colors

class var textColor: NSColor

The color to use for text.

class var placeholderTextColor: NSColor

The color to use for placeholder text in controls or text views.

class var selectedTextColor: NSColor

The color to use for selected text.

class var selectedTextBackgroundColor: NSColor

The color to use for the background of selected text.

class var keyboardFocusIndicatorColor: NSColor

The color to use for the keyboard focus ring around controls.

class var unemphasizedSelectedTextColor: NSColor

The color to use for selected text in an unemphasized context.

class var unemphasizedSelectedTextBackgroundColor: NSColor

The color to use for the text background in an unemphasized context.

