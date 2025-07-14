

- AppKit
- NSColor
-  controlColor 

Type Property

# controlColor

The color to use for the flat surfaces of a control.

macOS

``` source
class var controlColor: NSColor { get }
```

## Return Value

The system color used for the flat surfaces of a control. By default, the control color is a pattern color that will draw the ruled lines for the window background, which is the same as returned by windowBackgroundColor.

## Discussion

If you use controlColor assuming that it is a solid, you may have an incorrect appearance. You should use lightGray in its place.

## See Also

### Control Colors

class var controlAccentColor: NSColor

The user’s current accent color preference.

class var controlBackgroundColor: NSColor

The color to use for the background of large controls, such as scroll views or table views.

class var controlTextColor: NSColor

The color to use for text on enabled controls.

class var disabledControlTextColor: NSColor

The color to use for text on disabled controls.

class var currentControlTint: NSControlTint

The current system control tint color.

class var selectedControlColor: NSColor

The color to use for the face of a selected control—that is, a control that has been clicked or is being dragged.

class var selectedControlTextColor: NSColor

The color to use for text in a selected control—that is, a control being clicked or dragged.

class var alternateSelectedControlTextColor: NSColor

The color to use for text in a selected control.

class var scrubberTexturedBackground: NSColor

The patterned color to use for the background of a scrubber control.

