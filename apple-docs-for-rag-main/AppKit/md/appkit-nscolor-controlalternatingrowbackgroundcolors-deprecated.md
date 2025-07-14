

- AppKit
- NSColor
-  controlAlternatingRowBackgroundColors Deprecated

Type Property

# controlAlternatingRowBackgroundColors

An array containing the system specified background colors for alternating rows in tables and lists.

macOS 10.3–11.0Deprecated

``` source
class var controlAlternatingRowBackgroundColors: [NSColor] { get }
```

Deprecated

Use alternatingContentBackgroundColors instead.

## Return Value

An array of `NSColor` objects specifying the system colors used for rows in tables and lists. You should not assume the array will contain only two colors. For general information on system colors, see Accessing System Colors.

## See Also

### Deprecated Colors

class var alternateSelectedControlColor: NSColor

The system color used for the face of a selected control in a list or table.

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

