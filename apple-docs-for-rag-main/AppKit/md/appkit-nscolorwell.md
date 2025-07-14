

- AppKit
-  NSColorWell 

Class

# NSColorWell

A control that displays a color value and lets the user change that color value.

macOS

``` source
@MainActor
class NSColorWell
```

## Overview

An NSColorWell object lets people select colors from your interface. Incorporate this type of control if your app supports custom color selection. For example, a drawing app might include a color well to let someone choose the color to use when drawing. A color well control displays the currently selected color, and interactions with the color well display interfaces for selecting new colors.

When you create a color well programmatically or in Interface Builder, specify the appearance and interaction style you want. The color well supports color selection using a color picker popover or the system NSColorPanel object. When someone selects a new color in one of these interfaces, the color well updates its selected color to match. You can also provide your own color selection process using a custom action and update the color yourself.

## Topics

### Creating a Color Well

convenience init(style: NSColorWell.Style)

Creates a color well that adopts the specified appearance style.

### Managing the Selected Color

var color: NSColor

The currently selected color for the color well.

func takeColorFrom(Any?)

Changes the currently selected color to the color of the specified object.

var supportsAlpha: Bool

A Boolean value that determines whether the color picker supports alpha values.

### Configuring the Appearance

var colorWellStyle: NSColorWell.Style

The appearance and interaction style to apply to the color well.

enum Style

Constants that specify the appearance and interaction modes for a color well.

var image: NSImage?

The image to display on the button portion of a color well that adopts the expanded style.

var isBordered: Bool

A Boolean value that determines whether the color well has a border.

Deprecated

### Activating and Deactivating Color Wells

func activate(Bool)

Activates the color well, displays the color panel, and synchronizes the two UI elements.

var isActive: Bool

A Boolean value that indicates whether the color well is currently active.

func deactivate()

Deactivates the color well.

### Drawing Color Wells

func drawWell(inside: NSRect)

Draws the area inside the color well at the specified location without drawing borders.

### Customizing the Color Selection Behavior

var pulldownAction: Selector?

The action to perform when someone clicks in the color area of the color well.

var pulldownTarget: AnyObject?

The target object that defines the action you want to perform when someone interacts with the color well.

## Relationships

### Inherits From

- NSControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Color Selection

class NSColorPicker

An abstract superclass that implements the default color picking protocol.

class NSColorPickerTouchBarItem

A bar item that provides a system-defined color picker.

