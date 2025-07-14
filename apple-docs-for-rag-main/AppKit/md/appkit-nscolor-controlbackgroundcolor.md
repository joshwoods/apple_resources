

- AppKit
- NSColor
-  controlBackgroundColor 

Type Property

# controlBackgroundColor

The color to use for the background of large controls, such as scroll views or table views.

macOS

``` source
class var controlBackgroundColor: NSColor { get }
```

## Return Value

Do not use this color for drawing. Instead, use an NSVisualEffectView with the appropriate background material.

## Discussion

When applied to an NSBox object, this color supports Desktop Tinting in Dark Mode. With Desktop Tinting, the system modifies this color dynamically by incorporating some of the color from the underlying desktop image. The system does not apply this dynamic tinting effect to other types of views.

## See Also

### Control Colors

class var controlAccentColor: NSColor

The user’s current accent color preference.

class var controlColor: NSColor

The color to use for the flat surfaces of a control.

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

