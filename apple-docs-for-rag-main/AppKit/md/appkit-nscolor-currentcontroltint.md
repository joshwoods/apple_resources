

- AppKit
- NSColor
-  currentControlTint 

Type Property

# currentControlTint

The current system control tint color.

macOS

``` source
class var currentControlTint: NSControlTint { get }
```

## Return Value

The current system control tint.

## Discussion

An application can register for the currentControlTintDidChangeNotification notification to be notified of changes to the system control tint.

## See Also

### Related Documentation

init(for: NSControlTint)

Returns the color object specified by the given control tint.

Deprecated

### Control Colors

class var controlAccentColor: NSColor

The user’s current accent color preference.

class var controlColor: NSColor

The color to use for the flat surfaces of a control.

class var controlBackgroundColor: NSColor

The color to use for the background of large controls, such as scroll views or table views.

class var controlTextColor: NSColor

The color to use for text on enabled controls.

class var disabledControlTextColor: NSColor

The color to use for text on disabled controls.

class var selectedControlColor: NSColor

The color to use for the face of a selected control—that is, a control that has been clicked or is being dragged.

class var selectedControlTextColor: NSColor

The color to use for text in a selected control—that is, a control being clicked or dragged.

class var alternateSelectedControlTextColor: NSColor

The color to use for text in a selected control.

class var scrubberTexturedBackground: NSColor

The patterned color to use for the background of a scrubber control.

