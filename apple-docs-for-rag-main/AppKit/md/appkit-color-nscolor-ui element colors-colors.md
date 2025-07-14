

- AppKit
- Color
- NSColor
-  UI Element Colors 

API Collection

# UI Element Colors

Retrieve standard color objects for use with windows, controls, labels, text, selections and other content in your app.

## Overview

For design guidance, see Human Interface Guidelines.

## Topics

### Label Colors

class var labelColor: NSColor

The primary color to use for text labels.

class var secondaryLabelColor: NSColor

The secondary color to use for text labels.

class var tertiaryLabelColor: NSColor

The tertiary color to use for text labels.

class var quaternaryLabelColor: NSColor

The quaternary color to use for text labels and separators.

### Text Colors

class var textColor: NSColor

The color to use for text.

class var placeholderTextColor: NSColor

The color to use for placeholder text in controls or text views.

class var selectedTextColor: NSColor

The color to use for selected text.

class var textBackgroundColor: NSColor

The color to use for the background area behind text.

class var selectedTextBackgroundColor: NSColor

The color to use for the background of selected text.

class var keyboardFocusIndicatorColor: NSColor

The color to use for the keyboard focus ring around controls.

class var unemphasizedSelectedTextColor: NSColor

The color to use for selected text in an unemphasized context.

class var unemphasizedSelectedTextBackgroundColor: NSColor

The color to use for the text background in an unemphasized context.

### Content Colors

class var linkColor: NSColor

The color to use for links.

class var separatorColor: NSColor

The color to use for separators between different sections of content.

class var selectedContentBackgroundColor: NSColor

The color to use for the background of selected and emphasized content.

class var unemphasizedSelectedContentBackgroundColor: NSColor

The color to use for selected and unemphasized content.

### Menu Colors

class var selectedMenuItemTextColor: NSColor

The color to use for the text in menu items.

### Table Colors

class var gridColor: NSColor

The color to use for the optional gridlines, such as those in a table view.

class var headerTextColor: NSColor

The color to use for text in header cells in table views and outline views.

class var alternatingContentBackgroundColors: [NSColor]

The colors to use for alternating content, typically found in table views and collection views.

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

### Window Colors

class var windowBackgroundColor: NSColor

The color to use for the window background.

class var windowFrameTextColor: NSColor

The color to use for text in a window’s frame.

class var underPageBackgroundColor: NSColor

The color to use in the area beneath your window’s views.

### Highlights and Shadows

class var findHighlightColor: NSColor

The highlight color to use for the bubble that shows inline search result values.

class var highlightColor: NSColor

The color to use as a virtual light source on the screen.

class var shadowColor: NSColor

The color to use for virtual shadows cast by raised objects on the screen.

### Deprecated Colors

class var alternateSelectedControlColor: NSColor

The system color used for the face of a selected control in a list or table.

Deprecated

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

### Fill Colors

class var quaternarySystemFill: NSColor

class var quinaryLabel: NSColor

class var quinarySystemFill: NSColor

class var secondarySystemFill: NSColor

class var systemFill: NSColor

class var tertiarySystemFill: NSColor

class var textInsertionPointColor: NSColor

## See Also

### Getting and Creating Colors

Standard Colors

Retrieve the standard color objects for common colors like red, blue, green, black, white, and more.

Color Creation

Load colors from asset catalogs, and create colors from raw component values, such as those used by grayscale, RGB, HSB, and CMYK colors.

