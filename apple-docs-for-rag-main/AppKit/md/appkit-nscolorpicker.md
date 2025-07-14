

- AppKit
-  NSColorPicker 

Class

# NSColorPicker

An abstract superclass that implements the default color picking protocol.

macOS

``` source
class NSColorPicker
```

## Overview

The NSColorPickingDefault and NSColorPickingCustom protocols define a way to add color pickers (custom user interfaces for color selection) to the color panel.

## Topics

### Initializing the Color Picker Object

init?(pickerMask: Int, colorPanel: NSColorPanel)

Initializes the color picker with the specified color panel and color picker mode mask.

### Getting the Color Panel

var colorPanel: NSColorPanel

The color panel instance that owns the color picker.

### Adding Button Images

func insertNewButtonImage(NSImage, in: NSButtonCell)

Sets the image used for the specified button cell.

var provideNewButtonImage: NSImage

The button image used by the color picker.

### Setting the Mode

func setMode(NSColorPanel.Mode)

Overriden to set the color picker’s mode.

### Managing Color Lists

func attachColorList(NSColorList)

Overriden to attach a color list to a color picker.

func detachColorList(NSColorList)

Overriden to detach a color list from a color picker.

### Responding to View Changes

func viewSizeChanged(Any?)

Overriden to respond to a size change.

### Customizing the Color Picker

var buttonToolTip: String

The tool tip that is shown when the mouse cursor is over the color picker’s button image.

var minContentSize: NSSize

The minimum content size.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSColorPickingDefault
- NSObjectProtocol

## See Also

### Color Selection

class NSColorWell

A control that displays a color value and lets the user change that color value.

class NSColorPickerTouchBarItem

A bar item that provides a system-defined color picker.

