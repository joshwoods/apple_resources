

- AppKit
- NSColor
-  alternateSelectedControlColor Deprecated

Type Property

# alternateSelectedControlColor

The system color used for the face of a selected control in a list or table.

macOS 10.2–11.0Deprecated

``` source
class var alternateSelectedControlColor: NSColor { get }
```

Deprecated

Use selectedContentBackgroundColor instead.

## Return Value

The system color used for the face of a selected control—a control being clicked or dragged. This color is used in lists and tables. For general information about system colors, see Accessing System Colors.

## Discussion

This color is the table and list view equivalent to the selectedControlColor color, which is used for controls in other views.

For general information about system colors, see Accessing System Colors.

## See Also

### Related Documentation

class var alternateSelectedControlTextColor: NSColor

The color to use for text in a selected control.

Color Programming Topics

class var selectedControlColor: NSColor

The color to use for the face of a selected control—that is, a control that has been clicked or is being dragged.

### Deprecated Colors

class var controlAlternatingRowBackgroundColors: [NSColor]

An array containing the system specified background colors for alternating rows in tables and lists.

Deprecated

class var controlHighlightColor: NSColor

The system color used for the highlighted bezels of controls.

Deprecated

class var controlLightHighlightColor: NSColor

The system color used for light highlights in controls.

Deprecated

class var controlShadowColor: NSColor

The system color used for the shadows dropped from controls.

Deprecated

class var controlDarkShadowColor: NSColor

The system color used for the dark edge of the shadow dropped from controls.

Deprecated

class var headerColor: NSColor

The system color used as the background color for header cells in table views and outline views.

Deprecated

class var knobColor: NSColor

The system color used for the flat surface of a slider knob that hasn’t been selected.

Deprecated

class var selectedKnobColor: NSColor

The system color used for the slider knob when it is selected.

Deprecated

class var scrollBarColor: NSColor

The system color used for scroll “bars”—that is, for the groove in which a scroller’s knob moves

Deprecated

class var secondarySelectedControlColor: NSColor

The color used for selected controls in non-key views.

Deprecated

class var selectedMenuItemColor: NSColor

The color to use for the face of selected menu items.

Deprecated

class var windowFrameColor: NSColor

The system color used for window frames, except for their text.

Deprecated

