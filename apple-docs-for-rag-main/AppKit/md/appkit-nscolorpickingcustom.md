

- AppKit
-  NSColorPickingCustom 

Protocol

# NSColorPickingCustom

A set of methods that provides a way to add color pickers—custom user interfaces for color selection—to an app’s color panel.

macOS

``` source
protocol NSColorPickingCustom : NSColorPickingDefault
```

## Overview

NSColorPickingCustom works with the NSColorPickingDefault protocol—which provides basic behavior for a color picker—to enable custom color pickers.

Note

This protocol must be implemented by a custom picker, or an error will occur.

## Topics

### Configuring Color Pickers

func setColor(NSColor)

Adjusts the receiver to make the specified color the currently selected color.

**Required**

### Getting Color Picker Information

func currentMode() -> NSColorPanel.Mode

Returns the receiver’s current mode (or submode, if applicable).

**Required**

func supportsMode(NSColorPanel.Mode) -> Bool

Returns a Boolean value indicating whether or not the receiver supports the specified picking mode.

**Required**

### Displaying Color Pickers

func provideNewView(Bool) -> NSView

Returns the view containing the receiver’s user interface.

**Required**

## Relationships

### Inherits From

- NSColorPickingDefault

## See Also

### Color Panels

class NSColorPanel

A standard user interface for selecting color in an app.

protocol NSColorPickingDefault

A set of methods that provides basic behavior for a color picker.

class NSColorPicker

An abstract superclass that implements the default color picking protocol.

